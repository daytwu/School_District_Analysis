# School_District_Analysis

## Overview of the school district analysis: Explain the purpose of this analysis.

## Results: Using bulleted lists and images of DataFrames as support, address the following questions.

### How is the district summary affected?


Before Cleaning

<img width="695" alt="District_Summary_before_cleaning" src="https://user-images.githubusercontent.com/68725398/95883284-c2af3200-0d48-11eb-89b5-d325101ad11e.png">



After Cleaning

<img width="692" alt="District_Summary_after_cleaning" src="https://user-images.githubusercontent.com/68725398/95883331-ccd13080-0d48-11eb-924b-2a1318c21746.png">

The district summary is affected in that all the metrics other than Average Reading Score had dropped 0.1 to 0.3 points. % Overall Passing was the biggest drop, at 0.3 points, since it factors in both the % Passing Math and % Passing Reading.


### How is the school summary affected?

Before Cleaning

<img width="738" alt="Per_School_Summary_before_cleaning" src="https://user-images.githubusercontent.com/68725398/95883706-3cdfb680-0d49-11eb-82a2-a71d3893a7b7.png">

After Cleaning

<img width="744" alt="Per_School_Summary_after_cleaning" src="https://user-images.githubusercontent.com/68725398/95883713-3f421080-0d49-11eb-8575-aec04ae159cd.png">

The school summary's change was more noticeable in that the metrics was not diluted by other schools like the district summary was. In this summary, Thomas High School had a more noticeable difference in which all the metrics dropped (including Average Reading Score). % Overall Passing dropped the most with a .31 points drop with % Passing Reading in the second with a .29 point drop.

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Replacing the ninth graders' math and reading score had lowered Thomas High School's performance standing if comparing to itself only. Thomas High School's performance relative to the other schools in this district has not been affected much. The aforementioned .31 point drop in % Overall Passing did not lower it enough to drop from the Top 5 Schools dataframe as it is still .04 points higher than the school right below Thomas High School, which is Griffin High School at 90.59.


### How does replacing the ninth-grade scores affect the following:

- Math and reading scores by grade

Before Cleaning

![math_and_reading_avg_by_grade_before_cleaning](https://user-images.githubusercontent.com/68725398/95907868-3a418900-0d6a-11eb-8f10-260d4f3615a0.png)


After Cleaning

![math_and_reading_avg_by_grade_after_cleaning](https://user-images.githubusercontent.com/68725398/95907876-3ada1f80-0d6a-11eb-9c2d-0777d5fa8a65.png)

Although this was not specificly requested as a metric, we can find the overall grade average for both math and reading when we group the school_data_complete_df by grade. The only data that was replaced was the ninth-grade's reading and math scores, so the only grade that has any noticeable change would be 9th grade. 

Looking at the above series for the math and reading average, the drop is consistent with the rest of the dataframes when it comes to looking at things from a per school summary perspective or as a whole in the district summary. Math average seems to be have a bigger drop compared to Reading average, with a .2 point drop for math compared to a .08 point drop for reading.

- Scores by school spending

Before Cleaning

![Spending_summary_before_cleaning](https://user-images.githubusercontent.com/68725398/95911170-1df41b00-0d6f-11eb-894e-305f0a2b5387.png)

After Cleaning

![Spending_summary_after_cleaning](https://user-images.githubusercontent.com/68725398/95911175-1f254800-0d6f-11eb-8bd2-0eafb64e40ce.png)

Here we have two dataframes for data categorized by the school spending ranges (per student). Thomas High School falls under the $630-644 range, so this will be what section that gets focus. Among the listed metrics here, all categories received a drop in points except for Average Reading Score, which went up by .01 point. This shows that replacing the 9th Grade Reading scores actually brought up the average of all schools within the $630-644 spending range, unlike the other categories.

- Scores by school size

Before Cleaning

<img width="558" alt="Size_summary_before_cleaning" src="https://user-images.githubusercontent.com/68725398/95942989-9d570e00-0db2-11eb-9865-ebd5b2441850.png">

After Cleaning

<img width="557" alt="Size_summary_after_cleaning" src="https://user-images.githubusercontent.com/68725398/95942994-a1832b80-0db2-11eb-82d4-9ae94e6ca1fa.png">

- Scores by school type

Summary: Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
