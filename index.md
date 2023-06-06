# Lab Report 5 - Debugging Scenario & Reflection (Week 10)
## Part 1: Debugging Scenario
This section emulates an EdStem post where a student is seeking help with debugging.
1. Below is the content of the student's post:

> What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?
> I'm using my terminal connected to my ieng6 account.

> Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.
Seeing: 
```
[cs15lsp23lh@ieng6-201]:grader-skill-demo2:102$ bash grade.sh https://github.com/ucsd-cse15l-s23/list-methods-nested
Cloning into 'student-submission'...
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 4 (delta 0), reused 4 (delta 0), pack-reused 0
Receiving objects: 100% (4/4), done.
Finished cloning
grade.sh: line 10: FILE_PATH: command not found
ListExamples.java not found
Score: 0/4
```

> Expected to see: it searches for ListExamples.java anywhere in the student submission, find the ListExamples.java, grade the student's submission, and reports that all tests pass.


> Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.
> 1. failure-inducing input: `FILE_PATH =$(find student-submission -name "ListExamples.java")`.
> 2. Command before the failure line in the bash script:
```
CPATH='.:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar'
rm -rf student-submission
Im -rf grading-area
mkdir grading-area
git clone $1 student-submission
echo 'Finished cloning'
```
2. Next is the response from a TA:
> The line you got an error in is line 10, which reads "FILE_PATH: command not found". This is because Bash interprets "FILE_PATH" as a separate command instead of a variable. To fix it, remove the space between "FILE_PATH" and "=", as this is different from how common programming languages function. It's important to note this.

3. The terminal output after the sutdent fixed the bug:
```
[cs15lsp23lh@ieng6-201]:grader-skill-demo2:100$ bash grade.sh https://github.com/ucsd-cse15l-s23/list-methods-nested
Cloning into 'student-submission'...
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 4 (delta 0), reused 4 (delta 0), pack-reused 0
Receiving objects: 100% (4/4), done.
Finished cloning
ListExamples.java found

--------------
| Score: 4/4 |
--------------
```

The bug occurred because the student added an extra space between the variable "FILE_PATH" and "=". This is an error, as when we define a variable in bash script it should not have any extra spaces between the variable and "=". Otherwise, bash will interpret the variable as a separate command and thus produce the error "ListExamples.java not found".

4. The setup info:
The file & directory are actually the modification of the repo of skill demo 2: https://github.com/ucsd-cse15l-s23/grader-skill-demo2.

- The file & directory structure needed: 
files: GradeServer.java, Server.java, TestListExamples.java, grade.sh. 
directory: a lib for junit test.

- The content of each file before fixing the bug: 
GradeServer.java and Server.java are exactly the same as what's in the repo. 

The content of TestListExamples.java:
```
import static org.junit.Assert.*;
import org.junit.*;
import java.util.Arrays;
import java.util.List;

class IsMoon implements StringChecker {
  public boolean checkString(String s) {
    return s.equalsIgnoreCase("moon");
  }
}

public class TestListExamples {

  @Test(timeout = 500)
  public void testMergeRightEnd() {
    List<String> left = Arrays.asList("a", "c", "e");
    List<String> right = Arrays.asList("b", "e", "h");
    List<String> merged = ListExamples.merge(left, right);
    List<String> expected = Arrays.asList("a", "b", "c", "e", "e", "h");
    assertEquals(expected, merged);
  }

  @Test(timeout = 500)
  public void testMergeLeftEnd() {
    List<String> left = Arrays.asList("a", "c", "z");
    List<String> right = Arrays.asList("b", "d");
    List<String> merged = ListExamples.merge(left, right);
    List<String> expected = Arrays.asList("a", "b", "c", "d", "z");
    assertEquals(expected, merged);
  }

  @Test(timeout = 500)
  public void testFilterSingle() {
    List<String> input = Arrays.asList("Moon", "MOO", "moo");
    List<String> expect = Arrays.asList("Moon");
    List<String> filtered = ListExamples.filter(input, new IsMoon());
    assertEquals(expect, filtered);
  }

  @Test(timeout = 500)
  public void testFilterMulti() {
    List<String> input = Arrays.asList("Moon", "MOO", "moon", "MOON");
    List<String> expect = Arrays.asList("Moon", "moon", "MOON");
    List<String> filtered = ListExamples.filter(input, new IsMoon());
    assertEquals(expect, filtered);
  }
}
```
The content of grade.sh:
```
CPATH='.:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar'

rm -rf student-submission
rm -rf grading-area

mkdir grading-area

git clone $1 student-submission
echo 'Finished cloning'

if [[ -f student-submission/ListExamples.java ]]
then
  echo 'ListExamples.java found'
else
  echo 'ListExamples.java not found'
  echo 'Score: 0/4'
  exit 1
fi

cp student-submission/ListExamples.java ./grading-area

cp TestListExamples.java grading-area/
cp -r lib grading-area/

cd grading-area

javac -cp $CPATH *.java

java -cp $CPATH org.junit.runner.JUnitCore TestListExamples > junit-output.txt

# The strategy used here relies on the last few lines of JUnit output, which
# looks like:

# FAILURES!!!
# Tests run: 4,  Failures: 2

# We check for "FAILURES!!!" and then do a bit of parsing of the last line to
# get the count
FAILURES=`grep -c FAILURES!!! junit-output.txt`


if [[ $FAILURES -eq 0 ]]
then
  RESULT_LINE=`grep "OK " junit-output.txt`
  PASSED=${RESULT_LINE:4:1}
  TOTAL=$PASSED
else
  # The ${VAR:N:M} syntax gets a substring of length M starting at index N
  # Note that since this is a precise character count into the "Tests run:..."
  # string, we'd need to update it if, say, we had a double-digit number of
  # tests. But it's nice and simple for the purposes of this script.

  # See, for example:
  # https://stackoverflow.com/questions/16484972/how-to-extract-a-substring-in-bash
  # https://www.gnu.org/savannah-checkouts/gnu/bash/manual/bash.html#Shell-Parameter-Expansion

  RESULT_LINE=`grep "Tests run:" junit-output.txt`
  COUNT=${RESULT_LINE:25:1}
  TOTAL=${RESULT_LINE:11:1}

  PASSED=$(echo "($TOTAL-$COUNT)" | bc)

  echo "JUnit output was:"
  cat junit-output.txt
fi

echo ""
echo "--------------"
echo "| Score: $PASSED/$TOTAL |"
echo "--------------"
echo ""

```
