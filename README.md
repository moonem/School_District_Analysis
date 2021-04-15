# School District Analysis
A school district data, having 15 high schools and 39170 students from 9th grade to 12th grade, has been analyzed to retrieve the district summary and school summary based on the average *math* and *reading* scores based on *spending per student*, *school size* and *school type* (e.g., charter or district schools).

## Results
  * How is the district summary affected?
    *  Originally the school district had a total of 39,170 students. Due to dispute in some of the exam scores from *Thomas High School* 9th grade students, the district put a hold on 9th grade scores (by putting *NaN* for that school's 9th grade scores). This affected the new student count (i.e., total student count became 38,709 from previous total of 39,170 students, after dropping 461 9th graders of Thomas High School), which might affect the calculation for average and percentages to determine various district metrics. Let's take a look at the district summary before and after exclusion of those 9th graders.
    
    ![district summary before](/Resources/district_summary_df_before.png)
    
    Fig. 1. District Summary (before)
    
    ![district summary after](/Resources/district_summary_after1.png)
    
    Fig. 2. District Summary (after) 
 
 From Figs. 1 and 2, it can be seen that there is no changes between the district summaries before and after ignoring *Thomas High School (THS)*'s 9th grade students, other than the *Total Studetns* count. The reason behind this indifference is that the 9th grader's average scores in both *math* and *reading* appeared to be very close (less than 1% difference) to the *THS*'s 10th to 12th grader's average in respective subjects. When *THS* 9th grader's scores have been replaced by *NaN*s, those scores and associated students were not counted in calculating average and percentages. Since the average without *THS 9th graders* (and percentages also) were nearly equal to that of including them,the district summary outcome remained almost the same. 
 
 * How is the school summary affected?
    *  As discussed in the previous paragraph, the school summary has been affcted due to exclusion of *THS* 9th grader's scores as expected. Following figs. 3 and 4 highlight the difference in percentage scores between before and after exclusion of *THS* 9th grader's scores. 

    ![school summary before](/Resources/per_school_summary_before.png)
    
    Fig. 3. Per School Summary (before)
    
    ![school summary after](/Resources/per_school_summary_after1.png)
    
    Fig. 4. Per School Summary (after) 
     
 * How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
  * As discussed earlier, replacing the ninth graders’ math and reading scores didn't affect *Thomas High School*’s performance relative to the other schools because the replaced 9th grader's average score was nearly similar to the other grade students in *Thomas High School*.

 * How does replacing the ninth-grade scores affect the following:
    * Math and reading scores by grade
 ![math_reading before](/Resources/math_reading_by_grade_before.png)![after](/Resources/math_reading_by_grade_after.png)
    
    Fig. 5. *Math* and *Reading* scores (left) - before, (right) - after replacing the 9th grade scores.
    
    * Scores by school spending
      
      The scores by school spending had not been affected at all by the replacement of *THS* 9th grader's scores, because school budget and per student spending were not dependent on the individual or certain grade students' scores.
      
      ![spending summary](/Resources/spending_summary_after.png)  
    
    Fig. 6. Summary of scores by school spending remained the same after replacement of *THS*'s 9th grade scores.
    
    * Scores by school size
    
    ![size summary](/Resources/size_summary_after.png)  
    
    Fig. 7. Summary of scores by student numbers remained the same after replacement of *THS*'s 9th grade scores.
    
    * Scores by school type

    ![type summary](/Resources/type_summary_after.png)  
    
    Fig. 8. Summary of scores by school type also remained the same after replacement of *THS*'s 9th grade scores.
    
