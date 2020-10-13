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

- Scores by school spending

- Scores by school size

- Scores by school type

Summary: Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
