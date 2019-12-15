# School_District_Analysis
School District Analysis. Python

# Project Overview
# Analyze school district data on student funding and students’ standardized math and reading test scores to showcase trends on school performance. 
- Calculate the district summary.
- Calculate summary for each district school.
- Calculate the top 5 and bottom 5 performing schools.
- Calculate the average math score received by students in each grade level at each school.
- Calculate the average reading score received by students in each grade level at each school.
- Calculate the school performance based on the spending per student. 
- Calculate the school performance based on the size of the school.
- Calculate the school performance based on the type of school.

# Recourses

Data Source: schools_complete.csv and students_complete.csv
Software: Python 3.6.9:: Anaconda, Inc., Jupyter Notebook, 6.0.2, Visual Studio Code, 1.40.2

# Summary
- There were 15 school and 39,170 students in the data source. 

- The district summary:
	
|   | Total Schools | Total Students | Total Budget   | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing |
|---|---------------|----------------|----------------|--------------------|-----------------------|----------------|-------------------|-------------------|
| 0 | 15            | 39,170         | $24,649,428.00 | 79.0               | 81.9                  | 75             | 86                | 80                |

- The school summary:

|                       | School Type | Total Students | Total School Budget | Per Student Budget | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing |
|-----------------------|-------------|----------------|---------------------|--------------------|--------------------|-----------------------|----------------|-------------------|-------------------|
| Bailey High School    | District    | 4976           | $3,124,928.00       | $628.00            | 77.048432          | 81.033963             | 66.680064      | 81.933280         | 74.306672         |
| Cabrera High School   | Charter     | 1858           | $1,081,356.00       | $582.00            | 83.061895          | 83.975780             | 94.133477      | 97.039828         | 95.586652         |
| Figueroa High School  | District    | 2949           | $1,884,411.00       | $639.00            | 76.711767          | 81.158020             | 65.988471      | 80.739234         | 73.363852         |
| Ford High School      | District    | 2739           | $1,763,916.00       | $644.00            | 77.102592          | 80.746258             | 68.309602      | 79.299014         | 73.804308         |
| Griffin High School   | Charter     | 1468           | $917,500.00         | $625.00            | 83.351499          | 83.816757             | 93.392371      | 97.138965         | 95.265668         |
| Hernandez High School | District    | 4635           | $3,022,020.00       | $652.00            | 77.289752          | 80.934412             | 66.752967      | 80.862999         | 73.807983         |
| Holden High School    | Charter     | 427            | $248,087.00         | $581.00            | 83.803279          | 83.814988             | 92.505855      | 96.252927         | 94.379391         |
| Huang High School     | District    | 2917           | $1,910,635.00       | $655.00            | 76.629414          | 81.182722             | 65.683922      | 81.316421         | 73.500171         |
| Johnson High School   | District    | 4761           | $3,094,650.00       | $650.00            | 77.072464          | 80.966394             | 66.057551      | 81.222432         | 73.639992         |
| Pena High School      | Charter     | 962            | $585,858.00         | $609.00            | 83.839917          | 84.044699             | 94.594595      | 95.945946         | 95.270270         |
| Rodriguez High School | District    | 3999           | $2,547,363.00       | $637.00            | 76.842711          | 80.744686             | 66.366592      | 80.220055         | 73.293323         |
| Shelton High School   | Charter     | 1761           | $1,056,600.00       | $600.00            | 83.359455          | 83.725724             | 93.867121      | 95.854628         | 94.860875         |
| Thomas High School    | Charter     | 1635           | $1,043,130.00       | $638.00            | 83.418349          | 83.848930             | 93.272171      | 97.308869         | 95.290520         |
| Wilson High School    | Charter     | 2283           | $1,319,574.00       | $578.00            | 83.274201          | 83.989488             | 93.867718      | 96.539641         | 95.203679         |
| Wright High School    | Charter     | 1800           | $1,049,400.00       | $583.00            | 83.682222          | 83.955000             | 93.333333      | 96.611111         | 94.972222         |

- Top 5 and bottom 5 performing school:
   - The top 5 performing schools: 

|                     | School Type | Total Students | Total School Budget | Per Student Budget | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing |
|---------------------|-------------|----------------|---------------------|--------------------|--------------------|-----------------------|----------------|-------------------|-------------------|
| Cabrera High School | Charter     | 1858           | $1,081,356.00       | $582.00            | 83.061895          | 83.975780             | 94.133477      | 97.039828         | 95.586652         |
| Thomas High School  | Charter     | 1635           | $1,043,130.00       | $638.00            | 83.418349          | 83.848930             | 93.272171      | 97.308869         | 95.290520         |
| Pena High School    | Charter     | 962            | $585,858.00         | $609.00            | 83.839917          | 84.044699             | 94.594595      | 95.945946         | 95.270270         |
| Griffin High School | Charter     | 1468           | $917,500.00         | $625.00            | 83.351499          | 83.816757             | 93.392371      | 97.138965         | 95.265668         |
| Wilson High School  | Charter     | 2283           | $1,319,574.00       | $578.00            | 83.274201          | 83.989488             | 93.867718      | 96.539641         | 95.203679         |

   - The bottom 5 performing schools:

|                       | School Type | Total Students | Total School Budget | Per Student Budget | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing |
|-----------------------|-------------|----------------|---------------------|--------------------|--------------------|-----------------------|----------------|-------------------|-------------------|
| Rodriguez High School | District    | 3999           | $2,547,363.00       | $637.00            | 76.842711          | 80.744686             | 66.366592      | 80.220055         | 73.293323         |
| Figueroa High School  | District    | 2949           | $1,884,411.00       | $639.00            | 76.711767          | 81.158020             | 65.988471      | 80.739234         | 73.363852         |
| Huang High School     | District    | 2917           | $1,910,635.00       | $655.00            | 76.629414          | 81.182722             | 65.683922      | 81.316421         | 73.500171         |
| Johnson High School   | District    | 4761           | $3,094,650.00       | $650.00            | 77.072464          | 80.966394             | 66.057551      | 81.222432         | 73.639992         |
| Ford High School      | District    | 2739           | $1,763,916.00       | $644.00            | 77.102592          | 80.746258             | 68.309602      | 79.299014         | 73.804308         |


- Average math scores by grade for each school:

|                       | 9th  | 10th | 11th | 12th |
|-----------------------|------|------|------|------|
| Bailey High School    | 77.1 | 77.0 | 77.5 | 76.5 |
| Cabrera High School   | 83.1 | 83.2 | 82.8 | 83.3 |
| Figueroa High School  | 76.4 | 76.5 | 76.9 | 77.2 |
| Ford High School      | 77.4 | 77.7 | 76.9 | 76.2 |
| Griffin High School   | 82.0 | 84.2 | 83.8 | 83.4 |
| Hernandez High School | 77.4 | 77.3 | 77.1 | 77.2 |
| Holden High School    | 83.8 | 83.4 | 85.0 | 82.9 |
| Huang High School     | 77.0 | 75.9 | 76.4 | 77.2 |
| Johnson High School   | 77.2 | 76.7 | 77.5 | 76.9 |
| Pena High School      | 83.6 | 83.4 | 84.3 | 84.1 |
| Rodriguez High School | 76.9 | 76.6 | 76.4 | 77.7 |
| Shelton High School   | 83.4 | 82.9 | 83.4 | 83.8 |
| Thomas High School    | 83.6 | 83.1 | 83.5 | 83.5 |
| Wilson High School    | 83.1 | 83.7 | 83.2 | 83.0 |
| Wright High School    | 83.3 | 84.0 | 83.8 | 83.6 |


- Average reading scores by grade for each school:

|                       | 9th  | 10th | 11th | 12th |
|-----------------------|------|------|------|------|
| Bailey High School    | 81.3 | 80.9 | 80.9 | 80.9 |
| Cabrera High School   | 83.7 | 84.3 | 83.8 | 84.3 |
| Figueroa High School  | 81.2 | 81.4 | 80.6 | 81.4 |
| Ford High School      | 80.6 | 81.3 | 80.4 | 80.7 |
| Griffin High School   | 83.4 | 83.7 | 84.3 | 84.0 |
| Hernandez High School | 80.9 | 80.7 | 81.4 | 80.9 |
| Holden High School    | 83.7 | 83.3 | 83.8 | 84.7 |
| Huang High School     | 81.3 | 81.5 | 81.4 | 80.3 |
| Johnson High School   | 81.3 | 80.8 | 80.6 | 81.2 |
| Pena High School      | 83.8 | 83.6 | 84.3 | 84.6 |
| Rodriguez High School | 81.0 | 80.6 | 80.9 | 80.4 |
| Shelton High School   | 84.1 | 83.4 | 84.4 | 82.8 |
| Thomas High School    | 83.7 | 84.3 | 83.6 | 83.8 |
| Wilson High School    | 83.9 | 84.0 | 83.8 | 84.3 |
| Wright High School    | 83.8 | 83.8 | 84.2 | 84.1 |

- School performance based on the spending per student:

| Spending Ranges (Per Student) | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing |
|-------------------------------|--------------------|-----------------------|----------------|-------------------|-------------------|
| <$584                         | 83.5               | 83.9                  | 93             | 97                | 95                |
| $585-629                      | 81.9               | 83.2                  | 87             | 93                | 90                |
| $630-644                      | 78.5               | 81.6                  | 73             | 84                | 79                |
| $645-675                      | 77.0               | 81.0                  | 66             | 81                | 74                |

- School performance based on the size of the school:

| School Size        | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing |
|--------------------|--------------------|-----------------------|----------------|-------------------|-------------------|
| Small (<1000)      | 83.8               | 83.9                  | 94             | 96                | 95                |
| Medium (1000-2000) | 83.4               | 83.9                  | 94             | 97                | 95                |
| Large (2000-5000)  | 77.7               | 81.3                  | 70             | 83                | 76                |

- School performance based on the type of the school:

| School Type | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing |
|-------------|--------------------|-----------------------|----------------|-------------------|-------------------|
| Charter     | 83.5               | 83.9                  | 94             | 97                | 95                |
| District    | 77.0               | 81.0                  | 67             | 81                | 74                |

## Challenge Overview

- Remove the ninth-grade math and reading scores from Thomas High School and keep all other data associated with ninth-grade students and Thomas School intact.
- After removal of the data:
- Recalculate the district summary and answer how the district summary was affected.
 - Recalculate summary for each district school and answer how the school summary was affected.
 - Recalculate the top 5 and bottom 5 performing schools.
 - Recalculate the average math score received by students in each grade level at each school. Recalculate the average reading score received by students in each grade level at each school.
 - How does removing the ninth graders’ math and reading scores affect Thomas High School’s performance, relative to the other schools?
 - Recalculate the school performance based on the spending per student, the size of the school and the type of the school. 
 - How does removing the ninth-grade scores affect the Math and Reading Scores by Grade, Scores by School Spending, Scores by School Size, Scores by School Type? 

# Recourses
- Data Source: schools_complete.csv and students_complete.csv
- Software: Python 3.6.9:: Anaconda, Inc., Jupyter Notebook, 6.0.2, Visual Studio Code, 1.40.2

# Challenge Summary

- Cleaned the data by removing the professional prefixes or suffixes. 
- Removed the math and reading scores for ninth-grade students from Thomas High School.
- Recalculated the district and school summaries.
 - The district summary did not change significantly. The percentage of passing scores changed, but only by 1%. 

| 1 | Total Schools | Total Students | Total Budget   | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing |
|---|---------------|----------------|----------------|--------------------|-----------------------|----------------|-------------------|-------------------|
| 0 | 15            | 39,170         | $24,649,428.00 | 78.9               | 81.9                  | 74             | 85                | 79                |

- Recalculated the school performance 
 - The Thomas High School performance:

| Summary before removing the 9th grade math and reading scores | School Type | Total Students | Total School Budget | Per Student Budget | Average Math Score | Average Reading Score | % Passing Math | % Passing Reading | % Overall Passing |
|---------------------------------------------------------------|-------------|----------------|---------------------|--------------------|--------------------|-----------------------|----------------|-------------------|-------------------|
| Thomas High School                                            | Charter     | 1635           | $1,043,130.00       | $638.00            | 83.418349          | 83.848930             | 93.272171      | 97.308869         | 95.290520         |
| Summary after removing the 9th grade math and reading scores  |             |                |                     |                    |                    |                       |                |                   |                   |
| Thomas High School                                            | Charter     | 1635           | $1,043,130.00       | $638.00            | 83.350937          | 83.896082             | 66.911315      | 69.663609         | 68.287462         |
	
 - After removal of ninth-grade math and reading scores:
   - There was no significant change to the average of math and reading scores.
   - The percentage of math and reading passing scores, however, showed change from 95% to 68%. 
   - The new analysis shows that Thomas High School were in the bottom 5 performing schools, when before removal of 9th grade math and reading scores the Thomas High School was in the top 5 performing schools. 
   - As the Thomas High School overall performance has changed it also affected the other schools.
       - Wright High School moved to being in the top 5 performing schools.
       - Ford High School was no longer in the bottom 5 performing schools.
   - The data no longer shows any data for 9th graders from the Thomas High School.
       - It cannot be determined the average scores for 9th grade students from the Thomas High School in the math and reading scores by grade table.
   - There was no change to the scores by School Spending. There was not a significant change to the scores by School Size and Scores by School Type. 
       - There was a change for Medium size school performance, as the Thomas High School was in medium size school category. The average scores stayed the same, however the percentage of the passing scores decreased. 
       - The District school type scores did not change, however Charter school type performance decreased. 
- The removal of the ninth-grade math and reading scores from the Thomas High School decreased the overall passing percentage for the Thomas High School, taking the school from the top performing school to the bottom performing school. 


