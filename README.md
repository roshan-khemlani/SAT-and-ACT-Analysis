# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Standardized Testing, Statistical Summaries and Inference

### Overview

Problem Statement

What are the actions that can be taken and in which areas would investments best be made in order to 
increase participation rate among high school students in taking the SAT exams.

Executive Summary

The scope for this projects includes data covering participation rates and average test scores for students
taking the SAT and ACT exams during 2017 and 2018, particularly in the United States. This allows for a 
state-by-state comparison on the participation rate during these 2 years.

This project comprises of the following sections:
1. Importing and Cleaning of 2017 SAT & ACT Datasets
2. Importing and Cleaning of 2018 SAT & ACT Datasets
3. Exploratory Data Analysis on Different Deatures
4. Descriptive and Inferential Statistics
5. External Research to Understand the values in the dataset
6. Conclusion and Recommendations based on insights and research

### Datasets

|Feature|Type|Dataset|Description|Score Range(Min-Max)
|---|---|---|---|---|
|**state**|*object*|2017 ACT/SAT|States in the USA and District of Columbia|N/A
|**act17_rate**|*float*|2017 ACT|Mean Participation Rate for ACT in the respective state (Expressed in Decimal)|0 - 1
|**act17_eng**|*float*|2017 ACT|Mean English score in the ACT|1 - 36
|**act17_math**|*float*|2017 ACT|Mean Math score in the ACT|1 to 36
|**act17_read**|*float*|2017 ACT|Mean Reading score in the ACT|1 - 36
|**act17_science**|*float*|2017 ACT|Mean Science score in the ACT|1 - 36
|**act17_comp**|*float*|2017 ACT|Average score English, Math, Reading & Science|1 to 36
|**sat17_rate**|*float*|2017 SAT|Mean Participation Rate for SAT in the respective state (Expressed in Decimal)|0 - 1
|**sat17_ebrw**|*int*|2017 SAT|Mean Evidence-Based Reading and Writing score in the SAT|200 - 800
|**sat17_math**|*int*|2017 SAT|Mean Math score in the SAT|200 - 800
|**sat17_total**|*int*|2017 SAT|Mean Total score of Evidence-Based Reading and Writing & Math|400 - 1600


|Feature|Type|Dataset|Description|Score Range(Min-Max)
|---|---|---|---|---|
|**state**|*object*|2018 ACT/SAT|States in the USA and District of Columbia|N/A
|**act18_rate**|*float*|2018 ACT|Mean Participation Rate for ACT in the respective state (Expressed in Decimal)|0 - 1
|**act18_eng**|*float*|2018 ACT|Mean English score in the ACT|1 - 36
|**act18_math**|*float*|2018 ACT|Mean Math score in the ACT|1 to 36
|**act18_read**|*float*|2018 ACT|Mean Reading score in the ACT|1 - 36
|**act18_science**|*float*|2018 ACT|Mean Science score in the ACT|1 - 36
|**act18_comp**|*float*|2018 ACT|Total Mean score English, Math, Reading & Science|1 to 36
|**sat18_rate**|*float*|2018 SAT|Mean Participation Rate for SAT in the respective state (Expressed in Decimal)|0 - 1
|**sat18_ebrw**|*int*|2018 SAT|Mean Evidence-Based Reading and Writing score in the SAT|200 - 800
|**sat18_math**|*int*|2018 SAT|Mean Math score in the SAT|200 - 800
|**sat18_total**|*int*|2018 SAT|Total Mean score of Evidence-Based Reading and Writing & Math|400 - 1600


#### Provided Data

For this project, you'll have two provided datasets:

- [2017 SAT Scores](./data/sat_2017.csv)
- [2017 ACT Scores](./data/act_2017.csv)

These data give average SAT and ACT scores by state, as well as participation rates, for the graduating class of 2017.

You can see the source for the SAT data [here](https://blog.collegevine.com/here-are-the-average-sat-scores-by-state/), and the source for the ACT data [here](https://www.act.org/content/dam/act/unsecured/documents/cccr2017/ACT_2017-Average_Scores_by_State.pdf). **Make sure you cross-reference your data with your data sources to eliminate any data collection or data entry issues.**

#### Additional Data

2018 state-by-state average results and participation for the SAT are available in PDF reports [here](https://reports.collegeboard.org/sat-suite-program-results/state-results). 2018 ACT state-by-state mean composite scores and participation rates are [here](http://www.act.org/content/dam/act/unsecured/documents/cccr2018/Average-Scores-by-State.pdf) .

**This data has been compiled into CSV files which are also included in the *data* directory of this repo**

#### Outside Research

Based on my observations from the data sets above, I notice three states Illinois, Colorado and Rhode Island showing interesting trends in in their SAT participation rates.

Illinois, Colorado and Rhode Island has seen a 90%, 89% and 26% increase year over year from 2017 to 2018. This is mainly due to the new implementation by states which makes SAT an mandatory requirement for their high school children from 2017 onwards.

With this new mandate, high school children wont have to pay 138 dollars for the test, opening the door for children from low income families to participate in the tests. This can been in the scatter plot above, where I have included the median household income by state for 2017 and 2018. Point of the scatter plot is to see the correlation between high school children from low income families and the SAT participation rate. Year over year, we notice the income of each household plays an important factor in the participation rate of the SAT entrance exams as from the scatter plot above we see both 2017 and 2018 skewed to the right. The lower the household income the particpation rate will decline further. Unlike participation rates, most of the grade scores for both ACT and SAT test in the Histogram above are located closer to the mean in 2017 and 2018 with slight change in standard deviation.

As per 2018 ACT participation figures, Colorado and Illinois delcine 70% and 50% respectively. This shows how much influence state goverments can have over participation rates in either for college entrance exams. As per correlation matrix above, we could derive the both ACT and SAT participation rate is negatively correlated to the average score of the subjects and its total for both 2017 and 2018.

#### Conclusion
Base on the research above, we can see how much of influence the state goverment has over the participation rate of either SAT or ACT entrance exams.
There are currently 13 states who require their high school children to participate for ACT entrance exam and 20 states who states who require their high school children to participate for SAT entrance exam.
College board could work with state governments whose participation rates are below average for example South Dakota who have not made ACT an madatory requirment for their high school children to take the entrance exam but have a participation rate of 3%.
