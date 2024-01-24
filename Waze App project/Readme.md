# Unraveling Waze: Data-Driven Insights to Propel Growth
![image](https://github.com/jimi121/PYTHON-PROJECTS/blob/main/Waze%20App%20project/image.jpeg)
## Introduction

I explore the complexities of the Waze dataset in this dynamic data analytics research, using strong approaches to obtain insightful knowledge. The main goal is to comprehend and reduce monthly user churn on the Waze app, which is a vital task to support overall growth. Churn, which is determined by users deleting or stopping to use an app, is a crucial indicator that shapes the app's user base and level of happiness.

## Objective

The primary goals are as follows: first, thoroughly explore the dataset using inspection, A/B testing, and exploratory data analysis (EDA). Second, make use of the learned information to create plans that anticipate and prevent user attrition, which will increase user retention and improve customer happiness in general.

## Data Dictionary

| Field          | Description                                                                           |
|----------------|---------------------------------------------------------------------------------------|
|label |Binary target variable (“retained” vs “churned”) for if a user has churned anytime during the course of the month 	|
|sessions |	The number of occurrence of a user opening the app during the month |
|drives |	An occurrence of driving at least 1 km during the month |
|device |	The type of device a user starts a session with |
|total_sessions |A model estimate of the total number of sessions since a user has onboarded	|
|n_days_after_onboarding |The number of days since a user signed up for the app	|
|total_navigations_fav1 |Total navigations since onboarding to the user’s favorite place 1	|
|total_navigations_fav2 |Total navigations since onboarding to the user’s favorite place 2	|
|driven_km_drives |	Total kilometers driven during the month |
|duration_minutes_drives |	Total duration driven in minutes during the month |
|activity_days |Number of days the user opens the app during the month	|
|driving_days |Number of days the user drives (at least 1 km) during the month	|

# Insight from the Dataset

## Datset overview
- This dataset contains 82% retained users and 18% churned users.

- The dataset contains 12 unique variables with types including objects, floats, and integers; the label column is missing 700 
values with no indication that the omissions are non-random.

## Insights from User Behavior Analysis

- Churned users averaged ~3 more drives in the last month than retained users.

- Retained users used the app on over twice as many days as churned users in the last month.

- The median churned user drove ~200 more kilometers and 2.5 more hours during the last month than the median retained user.

- Churned users had more drives in fewer days, and their trips were farther and longer in duration. Perhaps this is suggestive of a user profile; our team will have to continue exploring! 

- The median user who churned drove 608 kilometers each day they drove last month, which is almost 250% the per-drive-day distance of retained users.

- Regardless of user churn, the users represented in this data drive a lot! It is probably safe to assume that this data does not represent typical drivers at large.

## Insights from the Exploratory Data Analysis

- The more times users used the app, the less likely they were to churn. While 40% of the users who didn't use the app at all last month churned, nobody who used the app 30 days churned.

- Number of driving days had a negative correlation with churn. Users who drove more days of the last month were less likely to churn.

- Users of all tenures from brand new to ~10 years were relatively evenly represented in the data.

- Nearly all the variables were either very right-skewed or uniformly distributed.

>  For the right-skewed distributions, this means that most users had values in the lower end of the range for that variable.

> For the uniform distributions, this means that users were generally equally likely to have values anywhere within the range for that variable.

- Several variables had highly improbable or perhaps even impossible outlying values, such as: driven_km_drives, activity_days and driving_days.

## Insight from A/B testing

- Based on the calculations, drivers who use an iPhone to interact with the application have a higher number of drives on average. 

- The t-test results concluded there is not a statistically significant difference in mean number of rides between iPhone users and Android users. 

# Recommendations:

#### User Engagement Strategies:

- Develop targeted engagement strategies for users who show signs of increased activity but are still prone to churn.
- Personalized notifications or rewards for frequent users could be used to promote persistent app usage.

#### Understanding Churned User Profiles:

- Conduct in-depth analysis to identify specific user profiles within the churned segment. Understanding their needs and pain points could lead to tailored retention strategies.

#### App Usability Improvements:

- To improve user experience and increase engagement, especially for those who might not be as active, think about improving the app's interface.

#### Data Quality Improvement:

- Address missing values in the label column and investigate the potential impact on analysis results. Ensure data accuracy and completeness for more reliable insights.

#### Regular Communication:

- Establish communication channels to interact with users, informing them about app updates, new features, or providing relevant content to maintain interest and usage frequency.

#### Further A/B Testing:

- While the initial A/B testing didn't reveal a statistically significant difference between iPhone and Android users, continue monitoring user behavior through ongoing A/B testing. Trends might change, and further insights could emerge over time.

# Conclusion

This comprehensive approach aims to not only understand user behavior but also implement targeted strategies to reduce churn and enhance user satisfaction, contributing to the sustained growth of the Waze app. This study provides stakeholders with a solid framework for strategic decision-making, directing initiatives to maximize user happiness and promote long-term growth.
