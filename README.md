# School_District_Analysis

## Overview of the school district analysis:

In this analysis, we are working with Maria, the Chief Data Scientist for the City School Systems. We are assigned multiple tasks to review and analyze the school data in multiple formats, such as fundings and standardized testing scores. These data will help Maria to look into any performance trends and drive discussions along with strategic decision. In turn, this will help the school board decide on budget allocations and decide on further funding priorities within the school system.

## Results:

### How is the district summary affected?


#### Before Cleaning

<img width="695" alt="District_Summary_before_cleaning" src="https://user-images.githubusercontent.com/68725398/95883284-c2af3200-0d48-11eb-89b5-d325101ad11e.png">

#### After Cleaning

<img width="692" alt="District_Summary_after_cleaning" src="https://user-images.githubusercontent.com/68725398/95883331-ccd13080-0d48-11eb-924b-2a1318c21746.png">

The district summary is affected in that all the metrics other than Average Reading Score had dropped 0.1 to 0.3 points. % Overall Passing was the biggest drop, at 0.3 points, since it factors in both the % Passing Math and % Passing Reading.


### How is the school summary affected?

#### Before Cleaning

<img width="738" alt="Per_School_Summary_before_cleaning" src="https://user-images.githubusercontent.com/68725398/95883706-3cdfb680-0d49-11eb-82a2-a71d3893a7b7.png">

#### After Cleaning

<img width="744" alt="Per_School_Summary_after_cleaning" src="https://user-images.githubusercontent.com/68725398/95883713-3f421080-0d49-11eb-8575-aec04ae159cd.png">

The school summary's change was more noticeable in that the metrics was not diluted by other schools like the district summary was. In this summary, Thomas High School had a more noticeable difference in which all the metrics dropped (including Average Reading Score). % Overall Passing dropped the most with a .31 points drop with % Passing Reading in the second with a .29 point drop.

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

#### Before Cleaning

<img width="749" alt="Top_5_before_cleaning" src="https://user-images.githubusercontent.com/68725398/95948174-1314a700-0dbe-11eb-90b7-a25df173aced.png">

#### After Cleaning

<img width="752" alt="Top_5_after_cleaning" src="https://user-images.githubusercontent.com/68725398/95948181-14de6a80-0dbe-11eb-8466-f6722b10ce35.png">

Replacing the ninth graders' math and reading score had lowered Thomas High School's performance standing if comparing to itself only. Thomas High School's performance relative to the other schools in this district has not been affected much. The aforementioned .31 point drop in % Overall Passing did not lower it enough to drop from the Top 5 Schools dataframe as it is still .04 points higher than the school right below Thomas High School, which is Griffin High School at 90.59.


### How does replacing the ninth-grade scores affect the following:

- Math and reading scores by grade

#### Before Cleaning

![math_and_reading_avg_by_grade_before_cleaning](https://user-images.githubusercontent.com/68725398/95907868-3a418900-0d6a-11eb-8f10-260d4f3615a0.png)


#### After Cleaning

![math_and_reading_avg_by_grade_after_cleaning](https://user-images.githubusercontent.com/68725398/95907876-3ada1f80-0d6a-11eb-9c2d-0777d5fa8a65.png)

Although data was not originally requested to be grouped by average for the entire grade originally (series were grouped by school_name then by grade), we can find the overall grade average for both math and reading when we group the school_data_complete_df by grade. The only data that was replaced was the ninth-grade's reading and math scores, so the only grade that has any noticeable change would be 9th grade. 

Looking at the above series for the math and reading average, the drop is consistent with the rest of the dataframes when it comes to looking at things from a per school summary perspective or as a whole in the district summary. Math average seems to be have a bigger drop compared to Reading average, with a .2 point drop for math compared to a .08 point drop for reading.

- Scores by school spending

#### Before Cleaning

![Spending_summary_before_cleaning](https://user-images.githubusercontent.com/68725398/95911170-1df41b00-0d6f-11eb-894e-305f0a2b5387.png)

#### After Cleaning

![Spending_summary_after_cleaning](https://user-images.githubusercontent.com/68725398/95911175-1f254800-0d6f-11eb-8bd2-0eafb64e40ce.png)

Here we have two dataframes for data categorized by the school spending ranges (per student). Thomas High School falls under the $630-644 range, so this will be what section that gets focus. Among the listed metrics here, all categories received a drop in points except for Average Reading Score, which went up by .01 point. This shows that replacing the 9th Grade Reading scores actually brought up the average of all schools within the $630-644 spending range, unlike the other categories.

- Scores by school size

#### Before Cleaning

<img width="558" alt="Size_summary_before_cleaning" src="https://user-images.githubusercontent.com/68725398/95942989-9d570e00-0db2-11eb-9865-ebd5b2441850.png">

#### After Cleaning

<img width="557" alt="Size_summary_after_cleaning" src="https://user-images.githubusercontent.com/68725398/95942994-a1832b80-0db2-11eb-82d4-9ae94e6ca1fa.png">

There are two notable changes in the above two dataframes for Size summaries. The first is that the Average Reading Score had went up after cleaning the 9th grade data which is consistent with the previous spending summary dataframes, only this time it was outlined by school size. The second being the drop on % Passing Reading, which although it is still a drop in points, it dipped enough to show difference if rounded up to the nearest tenth of the number. Most metric dataframes that was showcased here will not show a change if it was rounded up to a tenth of the number, with this being an noticeable exception for this scenario only.

- Scores by school type

#### Before cleaning

<img width="534" alt="Type_summary_before_cleaning" src="https://user-images.githubusercontent.com/68725398/95943734-9f21d100-0db4-11eb-9896-bca2bbdeb371.png">

#### After Cleaning

<img width="533" alt="Type_summary_after_cleaning" src="https://user-images.githubusercontent.com/68725398/95943741-a21cc180-0db4-11eb-9af4-b95fff83609f.png">

Thomas High School is a Charter School, so this will be the section to focus on. As with previous dataframes, Average Reading Score rose after the cleaning and all other categories dropped.

## Summary:

The four major changes appears to be that:

- 1) Average Reading Score has consistently went up when looking at dataframes categorized by spending, size or school types. This shows that the 9th grade reading scores were negatively affecting and dragging down this category.
- 2) Most other categories has had a noticeable drop if looking at it without formatting it to a tenth of a number, which can also mean that this change isn't impacting the metrics enough if not looking at stats so detailed.
- 3) % Overall Passing has a drop even with categories formatted to a tenth of a number in the district summary. This means that every all dataframes that shows a bit more detailed view of metrics can show the drop in points.
- 4) Average Math and Reading scores by grades will definitely be affected if all the data are turned into NaN.

