# School District Analysis
A school district data, having 15 high schools and 39170 students from 9th grade to 12th grade, has been analyzed to retrieve the ditrict summary and school summary based on the average *math* and *reading* scores based on *spending per student*, *school size* and *school type* (e.g., charter or district schools).

## Results
  * How is the district summary affected?
    *  Originally the school district has a total of 39,170 students. Due to dispute in some of the exam scores from *Thomas High School* 9th grade students, the district put a    hold on 9th grade scores (by putting *NaN* for that school's 9th grade scores). This affected the new student count (i.e., total student count became 38,709 from previous total of 39,170 students, after dropping 461 9th graders of Thomas High School), which might affect the calculation for average and percentages to determine various district metrics. Let's take a look at the district summary before and after exclusion of those 9th graders.
    
    ![district summary before] (Resources/district_summary_df_before.png)
    Fig. 1. District Summary (before)
    
    ![district summary after] (Resources/district_summary_after.png)
    Fig. 2. District Summary (after) 
