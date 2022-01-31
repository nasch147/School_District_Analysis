# PyCity Schools: A District-Wide Analysis of Reading and Math Standardized Test Scores in PyCity

## Overview and Background
![Load and Save Files](/Resources/load_save%20files.png)
I was tasked with analyzing standardized testing data for the PyCity School District.  Data regarding each of the 15 schoolss in the district, its type, the number of students attending, and each school's budget was provided via csv file. I also received data regarding each student, the high school they attend, their grade, and their reading and math scores.  The primary task is to examine trends in the enderlying data. However, this anlysis needed to be adjusted given suspected tampering with 9th drade test scores from Thomas High School.  The purpose of this analysis is to now examine the data following the removal of the expected scores from the set. Such factors such as school spending per capita, school type, grade of student, as well as a number of other factors were examined for their effect on test results in the distrct. 

### Removing corrupted scores

Using Python and the Pandas library, I was able to segregate corrupted scores using the. loc function, and replace those values with null, or, NaN figures so they would not skew the analysis. The results of this procedure can be seen in the images below for math and reading, respectively. The analysis on dsitrict scores was then reconducted and compared to the original result. 
![Load and Save Files](/Resources/load_save%20files.png)
![Load and Save Files](/Resources/load_save%20files.png)

## Results
- ### How is the district summary affected?
  - approximately 450 observations were removed from the set. Given the set comprises over 39,000 observations, this is unlikely to affect the analysis. The overall district summary above was not materially aletered from its original scores given the relatively smaller number of data points removed. 
- ### How is the school summary affected?
  - approximately 450 observations were removed from the set. Given the set comprises over 39,000 observations, this is unlikely to affect the analysis. However, the performance of Thomas High School 9th graders is not able to be benchmarked and ranked against other schools. 
- ### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
   - 9th grade scores were near the means for the High School and dropping those scores are unlikely to disrupt the analysis. 

- ### How does replacing the ninth-grade scores affect the following:

  - #### Math and reading scores by grade
   - the removal of math and reading scores from 9th graders at Thomas High School is evident in the images presented above. As previously mentioned, the removal of the data makes in impossible to measure these students against others in the district. 
  - #### Scores by school spending
   - ![Load and Save Files](/Resources/load_save%20files.png)
   - With less observations, per capita numbers from Thomas High School will be altered given that there are less students than in the original analysis. 
  - #### Scores by school size
   - ![Load and Save Files](/Resources/load_save%20files.png)
   - Though many observations were removed from the set. Thomas High School remains in the same size category as it did in the previous analysis. 
  - #### Scores by school type
   - ![Load and Save Files](/Resources/load_save%20files.png)
   - THomas high school was a charter school so the removal of the observations would change that category. 

## Summary
 - Removal of 450 test scores 
 - inability to compare THS 9th grade scores to others in the district
 - Slight changes in per capita metrics
 - Raw data read and cleaned without corrupting original data. 

