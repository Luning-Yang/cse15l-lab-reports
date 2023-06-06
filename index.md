# Lab Report 5 - Debugging Scenario & Reflection (Week 10)
## Debugging Scenario
This section minimics an EdStem post in which a student asks for a debugging help.
1. Below is the content of the student's post:

What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?
I'm using my terminal connected to my ieng6 account.

Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.
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

Expected to see:
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


Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.


