# Lab Report 3 - Researching Commands (Week 6)
The lab report showcases the implementation of the `grep` command with four different command-line options. The `grep` command is used on the directory located at https://github.com/ucsd-cse15l-s23/stringsearch-data.

1. `-i` would match the lines containing a specific word in a file. <br>
    Examples: <br>
    1.  The following example searches for and returns all lines which contain the string *hello* in the given file:<br>
        input: `grep -i "hello" stringsearch-data/technical/911report/chapter-1.txt`<br>
        output: ```At 10:39, the Vice President updated the Secretary on the air threat conference: Vice President: There's been at least three instances here where we've had reports of aircraft approaching Washington-a couple were confirmed hijack. And, pursuant to the President's instructions I gave authorization for them to be taken out. Hello?```
   2. The following example searches for and returns all lines which contain the string *using* in the given file:<br>
        input: `grep -i "using" stringsearch-data/technical/biomed/1468-6708-3-1.txt`<br>
        output: ```for all subjects using a baseline home interview, an
          report results using only the simpler definition.
          years, using validated methods presented elsewhere [ 20 ]
          for difference among BMI groups using confidence
        using either YHL or YOL as the outcome variable. Trials to
        evaluated using YHL, but not YOL. Trials to improve the
        the persons with partially estimated data, and using two
          be performed efficiently using either YOL or YHL as the
        measures of YHL. Using either YOL or YHL, however, we found
        'overweight' by the NHLBI guidelines. This suggests using```

2. `-r` will match and return the lines containing a specific word in **all** files under the given directory and its subdirectories. <br>
    Examples: <br>
    1.  The following example searches for and returns all lines which contain the string *vegetables* in all files under and the given directory and its subdirectories:<br>
        input: `grep -r "vegetables" stringsearch-data/technical/biomed` <br>
        output: ```stringsearch-data/technical/biomed/bcr583.txt:        were grouped according to type (fruits, vegetables, dairy,
stringsearch-data/technical/biomed/bcr583.txt:        consumption of fruits and vegetables was associated with a
stringsearch-data/technical/biomed/1472-6882-1-7.txt:        composed mostly of common fruits, vegetables, nuts, tubers,
stringsearch-data/technical/biomed/1472-6882-1-7.txt:          fruits, salads, raw vegetables, carrot juice, nuts,
stringsearch-data/technical/biomed/1472-6882-1-7.txt:          high intakes of fruits and vegetables resulted in high
stringsearch-data/technical/biomed/1471-2458-3-2.txt:          for brushing teeth, washing vegetables, consuming
stringsearch-data/technical/biomed/1471-2458-3-2.txt:          cleaning vegetables with tap water (yes, no) and
stringsearch-data/technical/biomed/1475-2891-2-1.txt:        non-refined cereals, fruits and vegetables, and it has a
stringsearch-data/technical/biomed/1475-2891-2-1.txt:          grain bread, pasta, brown rice, etc), vegetables (2 - 3
stringsearch-data/technical/biomed/1475-2891-2-1.txt:        legumes, and high in fibre, mostly from vegetables and
stringsearch-data/technical/biomed/1471-2458-3-11.txt:          cuts/meats, raw vegetables/fruits, raw oysters/shellfish,
stringsearch-data/technical/biomed/1471-2458-3-11.txt:          [0.02, 0.48]) and raw or uncooked vegetables (OR [95%
stringsearch-data/technical/biomed/1471-2458-3-11.txt:          (i.e., meat, fruit, or vegetables), was significantly
stringsearch-data/technical/biomed/1471-2458-3-11.txt:        to oocysts in raw vegetables and in unpasteurized products
stringsearch-data/technical/biomed/1471-2458-3-11.txt:        vegetables [ 53 ] . Indeed, it is likely that acquisition```
    2.  The following example searches for and returns all lines which contain the string *cannot* in all files under and the given directory and its subdirectories:<br>
        input: `grep -r "fruit" stringsearch-data/technical/government` <br>
        output: ```stringsearch-data/technical/government/About_LSC/Strategic_report.txt:also witnessed the fruition of prior efforts.
stringsearch-data/technical/government/About_LSC/commission_report.txt:of fruits and vegetables of every kind and other perishable
stringsearch-data/technical/government/About_LSC/commission_report.txt:apples (4,428), vegetable harvesting (4,822), and fruit harvesting
stringsearch-data/technical/government/Env_Prot_Agen/final.txt:recently borne fruit, particularly recent agreements with Japan and
stringsearch-data/technical/government/Alcohol_Problems/DraftRecom-PDF.txt:screening were not as fruitful topics for research as how to screen
stringsearch-data/technical/government/Gen_Account_Office/July11-2001_gg00172r.txt:fruition.
stringsearch-data/technical/government/Media/Unusual_Woodburn.txt:lettuce and chile harvests from the Central Valley to the fruit and
stringsearch-data/technical/government/Media/Farm_workers.txt:tending and harvesting fruits and vegetables.``` 

3. `-v` would match all lines except the lines containing a specific word in a file. <br>
    1. The following example searches for and returns all lines which do **not** contain the string *t* in the given file:<br>
    input: `grep -v "t" stringsearch-data/technical/biomed/1468-6708-3-1.txt` <br>
    output: ```elderly [ 9 ] .
        analyses based on years of life (YOL) or on YHL would
          Body mass index
          above.
          ] .
          primary analysis we used observed 7-year YOL and YHL when
          findings.
          peripheral vascular disease, or cerebrovascular disease),
          Analysis
          for difference among BMI groups using confidence
        smokers. Black women had a higher mean BMI and higher
        likely.
        for age, race, and previous smoking (columns 1 and 3), and
        under 20.
        same YOL.
        groups.
        YOL or YHL.
        Discussion
          YHL.
          person who is depressed because of a poor self-image
          of any differences in EVGFP.
        Conclusion
        None declared
        BMI Body mass index
        Scale
        poor?
        YOL Years of life```
        
    2. The following example searches for and returns all lines which do **not** contain the string *t* in the given file:<br>
    input: `grep -v "i" stringsearch-data/technical/plos/journal.pbio.0020001.txt` <br>
    output: 
    ```
            2002).
            Canada?
        programs.
        journals (
        Nature and
        to the top 11–20 journals. 
        In 
        A Long Road Yet to Travel
        world.
    ```
        
