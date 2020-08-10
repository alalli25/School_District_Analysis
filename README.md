# School District Analysis
Using Python and Pandas to analyze student test scores

## Overview of School District Analysis
### Purpose
The purpose of this project was to use python and the pandas library to view, manipulate, and organize school district & student data for a client, Maria. Maria is looking for me to provide a high-level snapshot of the district's key metrics, and an overview of the key metrics for each school, presented in data tables. After we completed our initial analysis, it was brought to my attention that the 9th grade reading and math grades for Thomas High School were fraudulent. I needed to use the loc method to remove the altered test scores and re-run my analysis.
#### My final output tables include:
- Top 5 and bottom 5 performing schools, based on the overall passing rate
- The average math score received by students in each grade level at each school
- The average reading score received by students in each grade level at each school
- School performance based on the budget per student
- School performance based on the school size 
- School performance based on the type of school

## School District Analysis Results & Summary
### Removing Thomas HS 9th Grade Results
To replace the Thomas High School 9th grade math and reading results, I created a loc, set my parameters to the data I wanted to change, and then changed the reading and math scores to "NaN".

***Thomas HS Post 9th Grade Data Removal***

![](/Resources/Screenshots/removed_9th.png)

#### Removing the data had the following implications:
- **District Summary** - The Total Schools, Total Students, Total Budget, and Avg Reading Score remain unchanged. The remaining metrics decreased.
- **School Summary** - The Avg Math and Reading scores decreased slightly, the % Passing Math, Reading, and Overall decreased dramatically *(Reference Thomas HS Summary Orig. vs Revised below)*


**Original**

![](/Resources/Screenshots/ThomasHS_Orig.png)

**Revised**

![](/Resources/Screenshots/ThomasHS.png)

- **Performance vs Other Schools** - Thomas High Schools' overall performance vs other schools decreased tremendously after removing the 9th grade reading and math grades. The school dropped from the second highest ranked school with a 90% overall passing grade to the eighth ranked school with a 65% overall passing grade.
- **Math and Reading Scores by Grade** - Only 9th grade data analysis was impacted by removing the Thomas High School 9th grade reading and math data. When looking at all 15 schools, the average reading score dropped 0.1% to 82.4% and average math score dropped 0.3% to 80.1%. *(Reference 9th Grade Analysis Tables below)*

**Original**

![](/Resources/Screenshots/summary_9th_orig.png)

**Revised**

![](/Resources/Screenshots/summary_9th.png)

- **Scores by School Spending** - Since Thomas High School is in the $630-644 spending range, only the % Passing Math, % Passing Reading and % Overall Passing for that spend range were negatively impacted. Each metric dropped roughly 6-7%. *(Reference School Spending Table below)*

**Revised School Spending**

![](/Resources/Screenshots/school_spending.png)

- **Scores by School Size** - Since Thomas High School is in the Medium (1000-2000) school size range, only the % Passing Math, % Passing Reading and % Overall Passing for that school size range were negatively impacted. Each metric dropped roughly 6-7%. *(Reference School Size Table below)*

**Revised School Size**

![](/Resources/Screenshots/school_size.png)

- **Scores by School Type** - Since Thomas High School is a charter school, only the % Passing Math, % Passing Reading and % Overall Passing for charter schools were negatively impacted. Each metric dropped roughly 3-4%. *(Reference School Type Table below)*

**Revised School Type**

![](/Resources/Screenshots/school_type.png)

### Removing Thomas HS 9th Grade Summary
Removing the Thomas HC 9th grade reading and math schools decreased many of the summarized metrics, meaning these removed scores included higher averages than the scores for the remaining schools. 
#### The four major changes were:
1. The medium (1000-2000) school size band had the highest passing percent for reading, math, & overall prior to removing the Thomas High School 9th grade scores. After the change, the small (<1000) school size band has the highest percent of passing students.
2. The spending per student band Thomas High School is in ($630-644) saw passing percent decrease significantly.
3. Overall 9th grade passing percentages decreased significantly.
4. Thomas High School dropped six positions after 9th grade scores were removed.

**Revised School Summary (Ranked)**

![](/Resources/Screenshots/school_summary.png)
