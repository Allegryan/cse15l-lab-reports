# Lab Report 3: Researching Commands
## `grep` command
**`grep -i` command**

Example 1:
```
$ grep -i "CDT" biomed/*.txt
biomed/1471-2091-3-23.txt:        proteins like Cdc6, Cdt1, MCMs, Cdc45 that are essential
biomed/1475-2875-1-5.txt:          Sense: (5') GAGGUAACCACGAAUGCGCdTdT (3')
biomed/1475-2875-1-5.txt:          Antisense: (5') GCGCAUUCGUGGUUACCUCdTdT (3')
biomed/gb-2002-3-10-research0055.txt:          provided for each example (ATR, GTR, CDT) must be copied
biomed/gb-2002-3-10-research0055.txt:          in the same folder before opening the CDT file with
biomed/gb-2002-3-10-research0055.txt:        CDT files ( Figure 6and Figure 7)) can be read by the
biomed/gb-2002-3-10-research0055.txt:        CDT file for Figure 6
biomed/gb-2002-3-10-research0055.txt:        CDT file for Figure 6
biomed/gb-2002-3-10-research0055.txt:        CDT file for Figure 7
biomed/gb-2002-3-10-research0055.txt:        CDT file for Figure 7
biomed/gb-2003-4-6-r37.txt:        data table (cdt) and gene tree correlations (gtr) files
biomed/gb-2003-4-6-r37.txt:        with associated atr, cdt and gtr files (Additional data
biomed/gb-2003-4-6-r37.txt:        the complete dataset for Figure 3, with associated atr, cdt
biomed/gb-2003-4-6-r37.txt:        files 13and 14) with associated atr, cdt and gtr files
```

Using `grep -i`, we were able to search the files for the given (case-insensitive) string -- in this case, "CDT". With this command, 
it'll help to be able to taking notes of patterns and repeated words or phrases that may appear in (text) files! 

Example 2:
```
$ grep -iE "CDT|YHL" biomed/*.txt
biomed/1468-6708-3-1.txt:        quality of life or years of healthy life (YHL) in the
biomed/1468-6708-3-1.txt:        differences in YHL would often require fewer subjects than
biomed/1468-6708-3-1.txt:        analyses based on years of life (YOL) or on YHL would
biomed/1468-6708-3-1.txt:          7 years after baseline. YHL is the number of years in
biomed/1468-6708-3-1.txt:          or active life expectancy [ 14 ] . We based YHL on
biomed/1468-6708-3-1.txt:          For this analysis we defined YHL as the number of
biomed/1468-6708-3-1.txt:          good, or good health (were 'healthy'). YHL ranges from 0
biomed/1468-6708-3-1.txt:          months, YHL has a reasonably continuous distribution. A
biomed/1468-6708-3-1.txt:          YHL from their age, sex, and health at the end of 3
biomed/1468-6708-3-1.txt:          . That article showed that estimated 4-year YOL and YHL
biomed/1468-6708-3-1.txt:          primary analysis we used observed 7-year YOL and YHL when
biomed/1468-6708-3-1.txt:          they were available, and observed 3-year YOL and YHL plus
biomed/1468-6708-3-1.txt:          4-year estimated YOL and YHL when they were not (about
biomed/1468-6708-3-1.txt:          The goal is to examine the association of YOL and YHL
biomed/1468-6708-3-1.txt:          follows. We regressed YOL and YHL first on age, age
biomed/1468-6708-3-1.txt:          group. Adjusted YHL was calculated in a similar manner.
biomed/1468-6708-3-1.txt:          plotted mean adjusted YOL and YHL against BMI, and tested
biomed/1468-6708-3-1.txt:          difference in mean YOL (or YHL) in two groups divided by
biomed/1468-6708-3-1.txt:        directions. Table 1shows the mean YOL and YHL (calculated
biomed/1468-6708-3-1.txt:        only 4.2 YHL of a maximum possible 7. We calculated some
biomed/1468-6708-3-1.txt:        lines: years of unhealthy life (YOL minus YHL) and years
biomed/1468-6708-3-1.txt:        lost to death (7 minus YOL). White women had the most YHL
biomed/1468-6708-3-1.txt:        were healthy (YHL/YOL, not shown); for whites, about 75%
biomed/1468-6708-3-1.txt:        unintended weight loss, YOL, YHL, years of unhealthy life,
biomed/1468-6708-3-1.txt:        YOL, YHL, years of unhealthy life, and years lost to death.
biomed/1468-6708-3-1.txt:        Blacks had significantly lower YOL and YHL than whites
biomed/1468-6708-3-1.txt:        We next examined the relationship of BMI to YOL and YHL.
biomed/1468-6708-3-1.txt:        Table 2presents the mean values of YOL and YHL, adjusted
biomed/1468-6708-3-1.txt:        covariates also made little difference for YHL (columns 3
biomed/1468-6708-3-1.txt:        the NHLBI guidelines, but had lower YOL and YHL than those
biomed/1468-6708-3-1.txt:        Figure 1is a plot of adjusted YOL and YHL by sex and
biomed/1468-6708-3-1.txt:        The lowermost two lines in Figure 1show mean YHL for
biomed/1468-6708-3-1.txt:        about 4.9 YHL. The YHL for underweight or obese women was
biomed/1468-6708-3-1.txt:        normal group. The relationship of BMI to YHL for men is
biomed/1468-6708-3-1.txt:        statistically significant. YHL was significantly higher for
biomed/1468-6708-3-1.txt:        the sexes had similar YHL in the underweight and obese
biomed/1468-6708-3-1.txt:        4.50 YHL compared to 4.92 for normal women, and the common
biomed/1468-6708-3-1.txt:        different YHL, implying that the effect size is also
biomed/1468-6708-3-1.txt:        about 93 women per treatment arm, if 7-year YHL were the
biomed/1468-6708-3-1.txt:        underweight to normal. YHL and YOL have similar effect
biomed/1468-6708-3-1.txt:        would be needed. For comparing obese to normal, only YHL
biomed/1468-6708-3-1.txt:        using either YHL or YOL as the outcome variable. Trials to
biomed/1468-6708-3-1.txt:        evaluated using YHL, but not YOL. Trials to improve the
biomed/1468-6708-3-1.txt:        YOL or YHL.
biomed/1468-6708-3-1.txt:        different ways of coding YHL. The only substantive change
biomed/1468-6708-3-1.txt:          people's YHL. This suggests that the development of
biomed/1468-6708-3-1.txt:          future guidelines should take YHL or other measures of
biomed/1468-6708-3-1.txt:          older women could be efficient if YHL (but not YOL) was
biomed/1468-6708-3-1.txt:          YHL, but not YOL. Clinical trials of weight modification
biomed/1468-6708-3-1.txt:          YHL.
biomed/1468-6708-3-1.txt:          be performed efficiently using either YOL or YHL as the
biomed/1468-6708-3-1.txt:          outcome measure. Both YOL and YHL would be clinically
biomed/1468-6708-3-1.txt:          superiority of YHL to YOL would probably hold in trials
biomed/1468-6708-3-1.txt:          EVGFP, on which YHL was based, might have missed some
biomed/1468-6708-3-1.txt:          be more sensitive to change in weight than EVGFP. If YHL
biomed/1468-6708-3-1.txt:          were based on such measures, the superiority of YHL to
biomed/1468-6708-3-1.txt:        found associations between YHL and obesity that were not
biomed/1468-6708-3-1.txt:        present in the mortality analysis, suggesting that YHL may
biomed/1468-6708-3-1.txt:        measures of YHL. Using either YOL or YHL, however, we found
biomed/1468-6708-3-1.txt:        YHL as the outcome measure in clinical trials involving
biomed/1468-6708-3-1.txt:        YHL Years of healthy life
biomed/1471-2091-3-23.txt:        proteins like Cdc6, Cdt1, MCMs, Cdc45 that are essential
biomed/1475-2875-1-5.txt:          Sense: (5') GAGGUAACCACGAAUGCGCdTdT (3')
biomed/1475-2875-1-5.txt:          Antisense: (5') GCGCAUUCGUGGUUACCUCdTdT (3')
biomed/gb-2002-3-10-research0055.txt:          provided for each example (ATR, GTR, CDT) must be copied
biomed/gb-2002-3-10-research0055.txt:          in the same folder before opening the CDT file with
biomed/gb-2002-3-10-research0055.txt:        CDT files ( Figure 6and Figure 7)) can be read by the
biomed/gb-2002-3-10-research0055.txt:        CDT file for Figure 6
biomed/gb-2002-3-10-research0055.txt:        CDT file for Figure 6
biomed/gb-2002-3-10-research0055.txt:        CDT file for Figure 7
biomed/gb-2002-3-10-research0055.txt:        CDT file for Figure 7
biomed/gb-2002-3-12-research0071.txt:          PGM1 , YHL0012w,
biomed/gb-2003-4-6-r37.txt:        data table (cdt) and gene tree correlations (gtr) files
biomed/gb-2003-4-6-r37.txt:        with associated atr, cdt and gtr files (Additional data
biomed/gb-2003-4-6-r37.txt:        the complete dataset for Figure 3, with associated atr, cdt
biomed/gb-2003-4-6-r37.txt:        files 13and 14) with associated atr, cdt and gtr files
```

Now for this example, we combined `-i` with `-E` in order to extend our expression. In this case, instead of just searching
for "CDT", it also searched for "YHL" (both case-insensitive) in the files. This helps in searching for multiple patterns
or repeated words/phrases at once!

For this command, I got help from this website: (https://www.gnu.org/savannah-checkouts/gnu/grep/manual/grep.html#Command_002dline-Options)

**`grep -n` command**

Example 1:
```
$ grep -n "CDT" biomed/*.txt
biomed/gb-2002-3-10-research0055.txt:750:          provided for each example (ATR, GTR, CDT) must be copied
biomed/gb-2002-3-10-research0055.txt:751:          in the same folder before opening the CDT file with
biomed/gb-2002-3-10-research0055.txt:790:        CDT files ( Figure 6and Figure 7)) can be read by the
biomed/gb-2002-3-10-research0055.txt:832:        CDT file for Figure 6
biomed/gb-2002-3-10-research0055.txt:833:        CDT file for Figure 6
biomed/gb-2002-3-10-research0055.txt:836:        CDT file for Figure 7
biomed/gb-2002-3-10-research0055.txt:837:        CDT file for Figure 7
```
`-n` is useful for finding the exact line numbers in which a given string is found. Note that in this case, as opposed to -i, 
the string is case-sensitive!

Example 2:
```
$ grep -n -C 2 "CDT" biomed/*.txt
biomed/gb-2002-3-10-research0055.txt-748-          the clustergram browser Treeview, which is available
biomed/gb-2002-3-10-research0055.txt-749-          online at no charge [ 10]. The three types of files
biomed/gb-2002-3-10-research0055.txt:750:          provided for each example (ATR, GTR, CDT) must be copied
biomed/gb-2002-3-10-research0055.txt:751:          in the same folder before opening the CDT file with
biomed/gb-2002-3-10-research0055.txt-752-          Treeview.
biomed/gb-2002-3-10-research0055.txt-753-
--
biomed/gb-2002-3-10-research0055.txt-788-        available. The literature profiles of Figures 6 and 7 (ATR
biomed/gb-2002-3-10-research0055.txt-789-        ( Figure 6and Figure 7), GTR ( Figure 6and Figure 7) and
biomed/gb-2002-3-10-research0055.txt:790:        CDT files ( Figure 6and Figure 7)) can be read by the
biomed/gb-2002-3-10-research0055.txt-791-        well-known open source dendrogram browser Treeview [
biomed/gb-2002-3-10-research0055.txt-792-        10].
--
biomed/gb-2002-3-10-research0055.txt-830-        Click here for additional data file
biomed/gb-2002-3-10-research0055.txt-831-        Additional data file 9
biomed/gb-2002-3-10-research0055.txt:832:        CDT file for Figure 6
biomed/gb-2002-3-10-research0055.txt:833:        CDT file for Figure 6
biomed/gb-2002-3-10-research0055.txt-834-        Click here for additional data file
biomed/gb-2002-3-10-research0055.txt-835-        Additional data file 10
biomed/gb-2002-3-10-research0055.txt:836:        CDT file for Figure 7
biomed/gb-2002-3-10-research0055.txt:837:        CDT file for Figure 7
biomed/gb-2002-3-10-research0055.txt-838-        Click here for additional data file
biomed/gb-2002-3-10-research0055.txt-839-
```

For this second implementation, we combined `-n` with `-C`, which allows us to see the "context" (or lines preceding the
found strings' line) for, in this example, 2 lines beforehand. This command helps in contextualizing lines that are found, seeing
as how, even if they aren't the exact lines that we may be looking for, said desired lines may need the context in order to
be fully understood.

For this command, I found help from this website: (https://man7.org/linux/man-pages/man1/grep.1.html)

**`grep -v` command**

Example 1:
```
$ grep -v "a" biomed/1468-6708-3-1.txt




        Introduction
        elderly [ 9 ] .



          Study
        



          ] .
          (for persons who were never in excellent, very good, or
          report results using only the simpler definition.
          findings.







        Results
        likely.
        from 25 to 29.9. The second column, which shows results
        under 20.
        groups.
        YOL or YHL.


        Discussion



          YHL.





        Conclusion
        'overweight' by the NHLBI guidelines. This suggests using


        Competing interests


        CESD Center for Epidemiologic Studies Depression
        poor?
```

`-v`, unlike `-i` enables us to be able to show only the lines that do *not* include the given string. This could be useful
if say, we need to filter out unnecessary information/lines, but we don't want to completely block out lines using `-i`, and would
rather view the lines again.

Example 2:
```
$ grep -vE "^\s*$" government/Media/5_Legal_Groups.txt 
5 Legal Groups at 1 Locale To Serve the February 3, 2002
Vulnerable
Salt Lake City Tribune
BY EDWARD MCDONOUGH
Five independent Salt Lake organizations that provide legal
services to the poor, ethnic minorities, seniors and people with
disabilities have joined together to acquire a west-side downtown
building where they will have their offices. The new Community
Legal Center at 205 N. 400 West is a project of "And Justice for
All," which, until this venture, has been a joint fund-raising
campaign by an alliance of the non-profit providers of free legal
services. "And Justice for All," which solicits donations primarily
from Utah lawyers and foundations, was the first joint fund-raising
campaign of legal services agencies in the country, and the
Community Legal Center is the first joint office project of public
service law groups.
The Legal Aid Society of Salt Lake, the Disability Law Center,
the Multi-Cultural Legal Center, the Senior Lawyer Volunteer
Project and Utah Legal Services will share the new facility, and
last Wednesday their board members were given a tour of the
Community Legal Center hosted by staff members of the five
agencies. All of the agencies can share the same reception area and
client waiting room. The building is close in, across the street
from West High and two blocks from the Gateway. It has its own
parking, something that's hard to find downtown and which has been
a problem for staff as well as clients. Owning and sharing the
building and not paying rent times five will save the non-profit
agencies about $375,000 each year. My assistant, Charity
Christenson, pointed out that the shared facility will also be
efficient for those needing legal services. No longer will a woman
desperate for a protective order, for example, have to run all over
town trying to find the right agency.
After the tour, we found Jaye Olafson at the cookies and
brownies reception on the first floor. Jaye and her husband, Erik,
own Tomax Technologies and were the sellers of the building. Jaye
explained how much of the renovation had been merely uncovering
what was already there. The hardwood floors, wooden ceilings and
brick and stone interior walls were all hidden behind coverings and
old paint. She loves the building, and they only moved out because
the business had outgrown the space. So they renovated the old
Sweet Candy Company building for Tomax. The Olafsons are delighted
with the new owners. The building had been like home, she
explained, and so it was important who would be living there. I
noted on the donor list that the couple, through Olafson Group, had
become one of the major supporters of the project.
Stewart Ralphs, the executive director of the Legal Aid Society,
explained that the Community Legal Center Campaign still has a long
ways to go, with a bit more than half of the $4 million projected
cost received so far. There still needed to be furnishings and
office equipment and such. He promised that they would be getting
in touch with us later on the subject.
```

In this example, I once again used the `-E` command in combination with `-v` in order to show all of the lines
that are not blank (i.e. do not contain 0 or more whitespace characters). This would help condense files and get rid
of unnecssary spaces and indenting.

For this command, I once again used this website: https://www.gnu.org/savannah-checkouts/gnu/grep/manual/grep.html#Command_002dline-Options

**`grep -R` command**

Example 1:
```
$ grep -R "incredible"
government/Media/Barnes_pro_bono.txt:aid program," said Gottlieb. "I take that as an incredible
government/Media/Poverty_Lawyers.txt:incredible inflation of private law firm salaries.
plos/journal.pbio.0020306.txt:        incredible ability of biology to make structures that could perhaps be incorporated in the
```

With the `-R` command, we are able to recursively search through the various subdirectories in a given directory. 
This is useful in that we no longer have to specify a subdirectory and/or limit ourselves to only searching a single
subdirectory!

Example 2:
```
$ grep -Rn "incredible"
government/Media/Barnes_pro_bono.txt:18:aid program," said Gottlieb. "I take that as an incredible
government/Media/Poverty_Lawyers.txt:40:incredible inflation of private law firm salaries.
plos/journal.pbio.0020306.txt:181:        incredible ability of biology to make structures that could perhaps be incorporated in the
```

Here, I combined `-R` with the aforementioned `-n` in order to not only search all of the subdirectories within the directory,
but also get the exact line number that the found string is found in within the file(s)!

For this command, I once again used this website: https://www.gnu.org/savannah-checkouts/gnu/grep/manual/grep.html#Command_002dline-Options

I also prompted ChatGPT for this one to provide me with an interesting implementation of `-R` in which case it suggested I
use it alongside `-n`!






