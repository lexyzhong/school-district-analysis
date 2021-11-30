# School District Analysis
## Overview of the school district analysis: 
The school board has requested for the following analyses to be performed and presented in a table format:
- district summary
- school summary
- top 5 and bottom 5 performing schools, based on the overall passing percentage
- average math score by grade level for each school
- average reading score by grade level for each school
- scores by school spending per student
- scores by school size
- scores by school type

After learning about the possible occurence of academic dishonesty at Thomas High School, the math and reading scores for all ninth grade students at this school were replaced with "NaN" (i.e. "not a number") and excluded from the calculations. The impact of excluding these scores on each of the aforementioned metrics will be discussed.

## Results: 
See ![PyCitySchools_Challenge.ipynb](https://github.com/lexyzhong/school-district-analysis/blob/main/PyCitySchools_Challenge.ipynb) for new analysis in which the ninth grade scores for Thomas High School were replaced.

See ![PyCitySchools.ipynb](https://github.com/lexyzhong/school-district-analysis/blob/main/PyCitySchools.ipynb) for original analysis.

### How is the district summary affected?
![district-summary.PNG](https://github.com/lexyzhong/school-district-analysis/blob/main/Resources/district-summary.PNG)

- "Total Schools" and "Total Budget" are unaffected by changes in the math and reading scores for ninth grade students at Thomas High School
- "Total Students" is unaffected as complete rows of student data were not removed
- "Average Math Score" decreased from 79.0 to 78.9
- "Average Reading Score" calculations were affected but the output remain unchanged
- "% Passing Math" decreased from 75.0% to 74.8%
- "% Passing Reading" decreased from 85.8% to 85.7%
- "% Overall Passing" decreased from 65.2% to 64.9%


### How is the school summary affected?
![school-summary.PNG](https://github.com/lexyzhong/school-district-analysis/blob/main/Resources/school-summary.PNG)

- For Thomas High School, the following changes occurred:
    - "Average Math Score" decreased from 83.418349 to 83.350937
    - "Average Reading Score" increased from 83.848930 to 83.896082
    - "% Passing Math" decreased from 93.272171% to 93.185690%
    - "% Passing Reading" decreased from 97.308869% to 97.018739%
    - "% Overall Passing" decreased from 90.948012% to 90.630324%

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
**Top 5 performing schools**
![top-5.PNG](https://github.com/lexyzhong/school-district-analysis/blob/main/Resources/top-5.PNG)

**Bottom 5 performing schools**
![bottom-5.PNG](https://github.com/lexyzhong/school-district-analysis/blob/main/Resources/bottom-5.PNG)

- School rankings were unaffected and Thomas High School remains the second best performing school in the district based on overall passing percentags

### How does replacing the ninth-grade scores affect the following:
#### Math and reading scores by grade
![math-scores-by-grade.PNG](https://github.com/lexyzhong/school-district-analysis/blob/main/Resources/math-scores-by-grade.PNG)

![reading-scores-by-grade.PNG](https://github.com/lexyzhong/school-district-analysis/blob/main/Resources/reading-scores-by-grade.PNG)

- math and reading scores for ninth grade students at Thomas High School are "nan" (not available) and other scores are unaffected
- 

#### Scores by school spending
![scores-by-spending.PNG](https://github.com/lexyzhong/school-district-analysis/blob/main/Resources/scores-by-spending.PNG)

- scores by school spending were not affected by replacing the ninth-grade scores
- the scores by school spending table suggests that increased spending does not increase student performance as schools that spent the highest (between $645-$675) per student performed worse in all metrics measured than schools that spent the least (<$584) per student 

#### Scores by school size
![scores-by-size.PNG](https://github.com/lexyzhong/school-district-analysis/blob/main/Resources/scores-by-size.PNG)

- scores by school size were not affected by replacing the ninth-grade scores
- scores by school size suggests that the school size correlates inversely with student performance as the largest schools (size 2000-5000 students) performed worse in all metrics measured than the smallest schools (<1000 students)

#### Scores by school type
![scores-by-type.PNG](https://github.com/lexyzhong/school-district-analysis/blob/main/Resources/scores-by-type.PNG)

- scores by school type were not affected by replacing the ninth-grade scores
- charter schools out-performed district schools in all metrics measured

## Summary:
After replacing the reading and math scores for the ninth grade students at Thomas High School with "NaN"s, the average math scores, the percentage passing math, the percentage passing reading, and overall passing percentage decreased at Thomas High School as well as for the district.
