# Project 1: Standardized Testing, Statistical Summaries and Inference


## Problem Statement 

The new format for the SAT was released in March 2016. The College Board seeks to track statewide participation and recommends where money is best spent to improve SAT participation rates.

My problem statement is:
How the College Board might work to increase the participation rate in Kansas?

## Executive Summary

### 2017 Data Import & Cleaning
There are two datasets, the first dataset is sat_2017. sat_2017 is a breakdown of the average SAT score (2017 cohort) in each United States (US) state according to the 2017 SAT Suite of Assessments Annual Report. 

sat_2017 consists of 51 rows by 5 columns. Each row represents an US state in relation to its individual (column): 

* SAT Participation Rate (string, in %) 
* Average Evidence-Based Reading and Writing Score (integer,out of 800)
* Average Math Score (integer,out of 800)
* Total Average Score (integer,out of 1600) 

The second dataset is act_2017. act_2017 is a breakdown of the average ACT score (2017 cohort) in each US state by subject. 

act_2017 consists of 52 rows by 7 columns. Each row represents an US state in relation to its individual (column):

* ACT Participation Rate (string, in %) 
* Average English Score (float)
* Average Math Score (float)
* Average Reading Score (float)
* Average Science Score (float)
* Average Composite Score (float,out of 36) 

### 2018 Data Import and Cleaning

There are two datasets, the first dataset is sat_2018. sat_2018 is a breakdown of the average SAT score (2018 cohort) in each United States (US) state according to the 2018 SAT Suite of Assessments Annual Report. 

sat_2018 consists of 51 rows by 5 columns. Each row represents an US state in relation to its individual (column): 

* SAT Participation Rate (string, in %) 
* Average Evidence-Based Reading and Writing Score (integer,out of 800)
* Average Math Score (integer,out of 800)
* Total Average Score (integer,out of 1600) 

The second dataset is act_2018. act_2018 is a breakdown of the average ACT score (2018 cohort) in each US state by subject. 

act_2018 consists of 52 rows by 3 columns. Each row represents an US state in relation to its individual (column):

* ACT Participation Rate (string, in %) 
* Average Composite Score (float,out of 36) 

### Exploratory Data Analysis

SAT 2017/18 State with Lowest Average Total:
* District of Columbia (2017)
* District of Columbia (2018)

SAT 2017/18 State with Highest Average Total:
* Minnesota (2017)
* Minnesota (2018)

ACT 2017/18 State with Lowest Composite:
* Nevada (2017)
* Nevada (2018)

ACT 2017/18 State with Highest Composite:
* New Hampshire (2017)
* Connecticut (2018)


### Data Visualization

There seems to be a moderate positive linear relationship between SAT 2017 total and SAT 2018 total. States that score well in SAT 2017, generally also scores well in 2018 vice-versa.

There seems to be a moderate positive linear relationship between ACT 2017 composite and ACT 2018 composite. States that score well in SAT 2017, generally also scores well in 2018 vice-versa.

SAT 2018 participation and SAT 2018 subjects ebrw, math, total are generally negatively correlated. This means higher participation leads to lower score, vice versa, lower participation leads to higher score.

### Descriptive and Inferential Statistics

All variables were not normally distributed and they were skewed.

It does not make sense to conduct statistical inference given these data. The dataset represents the participation and performance of all students across all US states. These data represents the population, not a sample. Satistical inference can only be made when we draw a sample from the population, we use the sample to make statistical inference on the population parameters. 

### Outside Research

Nearly 2 million US students in the class of 2018 took the SAT during high school, compared with 1.91 million who took the ACT. This is the largest number of students in a graduating class to take the SAT. College Board had been revising test and entering deals with numerous states and school system to give students exam. Two prominent states that switched to SAT were Colorado and Illinois. 

SAT had also introduced SAT School Day Program which allow students to take the test during school days, instead of during weekends. Income-eligible student can take the SAT for free with a fee waiver. 

SAT had launched a new version in 2016, which make the test more straightforward and approachable. 


## Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**state**|*object*|sat_2017/act_2017|State names that participated in SAT or ACT exam. Total 51 states.| 
|**participation**|*float*|sat_2017/act_2017/sat_2018/act_2018|Percentage of students who took part in SAT/ACT for the year 2017. (range:0-1).|
|**sat_17_ebrw**|*int*|sat_2017|Average score for SAT Evidence-Based Reading and Writing (range:200-800).|
|**sat_17_math**|*int*|sat_2017|Average score for SAT Math (range:200-800).|
|**sat_17_total**|*int*|sat_2017|Average total score for each state (range:400-1600).|
|**act_17_english**|*float*|act_2017|Average ACT English score for each state (range:1-36).|
|**act_17_math**|*float*|act_2017|Average ACT Math score for each state (range:1-36).|
|**act_17_reading**|*float*|act_2017|Average ACT Reading score for each state (range:1-36).|
|**act_17_science**|*float*|act_2017|Average ACT Science score for each state (range:1-36).|
|**act_17_composite**|*float*|act_2017|Average scaled total score for each state (range:1-36).|
|**sat_18_erbw**|*int*|sat_2018|Average score for SAT Evidence-Based Reading and Writing (range:200-800).|
|**sat_18_math**|*int*|sat_2018|Average score for SAT Math (range:200-800).|
|**sat_18_total**|*int*|sat_2018|Average total score for each state (range:400-1600).|
|**act_18_composite**|*float*|act_2018|Average scaled total score for each state (range:1-36).|

## Recommendations

Kansas is chosen to provide suggestions for College Board. Kansas has the lowest SAT participation rate among the states but has one of the higest SAT test score (See figure 4). Besides that, according to American School and University, Kansas was ranked top 6 in student to population ratio . This means that Kansas has a large student population (193,733). It would be a great boost if SAT can win Kansas over. Moreover, Kansas is a state sitting on the fence, it does not favour either SAT or ACT (See figure 1). My suggestions based on the marketing 4ps are as follows:

Product: Creating an equal platform for students to succeed 
- The current strategy for SAT is to increase participation rate. However, there is a strong negative correlation between participation rate and total score. This means that the more students participate the worse the total score. SAT could restructure its exam to better suit curriculums in Kansas and other states. For example, revising the tricky vocabulary section had proven to be a success. SAT could improve access to test materials, allocating resource to ease the financial burden of students. Besides that, SAT school day program could be extended to Kansas, making it easy for students to take the exam during school days instead on weekends. Giving students an equal platform to score well would be a better strategy than merely looking to increase participation rate. 

Price: Make SAT affordable to Kansas
- Kansas currently does not pay for students to take SAT exam.(See figure 2, Kansas is one of the grey states) This means that students will have to pay on their own for test preparation and actual test. Income eligible students could get the test fee and test prepation fees waived. It would be ideal for Kansas state to sponsor test fees for its students, SAT could provide a discount to entice Kansas. SAT could offer 2 subsequent free test for students in Kansas.  

Place: Ready support to students
- SAT could offer mock exams to 10th graders before they take the actual exam in 11th grade. Besides mock exam, more test prepartion material could be released at 10th grade so as to allow students to familiarise with SAT. Test prep material could be provided in schools and online so as to allow easy access to learning material for students. With more support, students will have better chance to score well and therefore more confident to take SAT. 

Promotion: Position SAT as a brand that help students to succeed 
- According to broadband search, 94.4% of Kansas residents have wireline internet available to them. Therefore, online promotion strategy would be ideal. Besides that, our target population are the schools and state council. They are the ones who decide on policies such as which test will be make mandatory. Therefore, getting the support of the traditonal media would be advantageous. Promote on creditable jornals would enhance the image of SAT. The brand message could be the varies strategies the SAT uses that help students succed, for instance the product, price and place mentioned above.  

### Future Data Collection Recommendations

1. The exact number of students in each state who took either SAT or ACT. Reason being, some state may have a very small participation percentage but the exact number of students might be higher than those states that have higher participation percentage because the state has many more students. 
2. The total number of students for the year in each state. Same reason as point 1. 
3. The population of each state and general demographics (Sample Social demographic data). Assess the student population to general population, some state may face ageing problem or low birth rate or low disposable income that might contribute to low participation or bias towards one test (ACT or ACT). 
4. The type of schools (Public or Private or district) that participated in SAT or ACT. Might show some trend on participation percentage and average score. 
5. Provide samples of student test scores instead of overall state average.  