# Lab Report 3 - Researching Commands (Week 6)
The lab report demonstrates the usage of the command `grep` with 4 different command-line options. The directory we use for `grep` is https://github.com/ucsd-cse15l-s23/stringsearch-data. 

1. `-i` would match the lines containing a specific word in a file. <br>
    Examples: <br>
    1.  The following example searches for and returns all lines which contain the word *hello* in the given file:<br>
        input: `grep -i "hello" stringsearch-data/technical/911report/chapter-1.txt`<br>
        output: `At 10:39, the Vice President updated the Secretary on the air threat conference: Vice President: There's been at least three instances here where we've had reports of aircraft approaching Washington-a couple were confirmed hijack. And, pursuant to the President's instructions I gave authorization for them to be taken out. Hello?`
   2. The following example searches for and returns all lines which contain the word *using* in the given file:<br>
        input: `grep -i "using" stringsearch-data/technical/biomed/1468-6708-3-1.txt`<br>
        output: `for all subjects using a baseline home interview, an
          report results using only the simpler definition.
          years, using validated methods presented elsewhere [ 20 ]
          for difference among BMI groups using confidence
        using either YHL or YOL as the outcome variable. Trials to
        evaluated using YHL, but not YOL. Trials to improve the
        the persons with partially estimated data, and using two
          be performed efficiently using either YOL or YHL as the
        measures of YHL. Using either YOL or YHL, however, we found
        'overweight' by the NHLBI guidelines. This suggests using`
