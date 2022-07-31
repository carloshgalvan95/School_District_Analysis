# School_District_Analysis
---
# Overview
Provide insight about performance trends and patterns. These insights will be used to informed discussions and strategic decisions at the school and district level. The objective is to analyze the data to provide information based in student funding and student standardized test scores as well as showcasing trends on school performance to inform the school board to make decisions regarding the school budgets and areas of improvement.

After running the analysis for all schools, evidence of academic dishonesty was found; specifically in reading and math grades for Thomas High School ninth graders. Although the school board does not know the full extent of the academic dishonesty, to be able to make informed decisions based on accurate information, the analysis will be run a second time replacing the grades for ninth graders at Thomas High School with **NaNs** to identify how these changes affected the overall analysis

# Results
---
## How is the district summary affected?
We can observe that, given the low number of students the data replaced represents, there are no noticeable changes between our first analysis and the new analysis made without Thomas High School ninth graders.

[SchoolSummary_wnans](https://github.com/carloshgalvan95/School_District_Analysis/blob/main/Resources/SchoolSummary_wnans.png)

[SchoolSummary_nonans](https://github.com/carloshgalvan95/School_District_Analysis/blob/main/Resources/SchoolSummary_nonans.png)

## How is the school summary affected?
The differences perceived from making this change start to be more noticeable when running this analysis. Given that the schools are analyzed and evaluated for the overall passing percentage or both reading and math, if we take 25% of the data, all the ninth graders, out of the equation, the results are obviously going to be rather inconclusive. 

School Summary with NaNs                   |  School Summary with no NaNs
:-------------------------:|:-------------------------:
![SchoolSummary_wnans](https://github.com/carloshgalvan95/School_District_Analysis/blob/main/Resources/SchoolSummary_wnans.png)  |  ![SchoolSummary_nonans](https://github.com/carloshgalvan95/School_District_Analysis/blob/main/Resources/SchoolSummary_nonans.png)

Top 5 Schools                  |  Lower 5 Schools
:-------------------------:|:-------------------------:
![top5](https://github.com/carloshgalvan95/School_District_Analysis/blob/main/Resources/top5_nonans.png)  |  ![low5](https://github.com/carloshgalvan95/School_District_Analysis/blob/main/Resources/low5_nonans.png)

We can see here that, if we take into consideration the full sample of total students for Thomas High School, we get very low numbers. But if we take it out of the equation the results can be misleading placing Thomas High School as one of the best performing schools.

## How does replacing the ninth-grade scores affect the following:
 ### -  Math and reading scores by grade
 There are no changes after running the analysis without the Thomas High School Ninth Graders given that the table generated is arranged by schools and grade, therefore, the only noticeable difference would be the “nan” at the 9th graders Thomas High School cell.
 
 ### - Scores by school spending
 We cannot see any noticeable differences here as well, in order to avoid analyzing misleading information, we would need to have or estimate the real scores for the ninth graders
 
 ### - Scores by school size
 ### - Scores by school type
 
 # Summary
 ---
 
 After running the analysis leaving out the grades for Thomas High School ninth-graders we notice a few changes in our metrics:
 
 1. First we must analyze and consider this information taking into account that the method that we used for running the new analysis is one of few different approaches we can take when doing exploratory data analysis and cleaning data as with all the other metods, dropping the rows, ignoring or replacing the values, it comes with a few caveats. The data is misleading, given the fact that we are not dropping the rows of students, the analysis is still done with the total number of students of Thomas High School leading to very low metrics and percentages for the other students. If we instead decide on ignoring those students, the overall passing percentages are probably going to be higher than the real percentage.
 
 2. The scope of the sample is quite large 