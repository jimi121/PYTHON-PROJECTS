# 🚗 Waze User Churn Analysis: Insights for Growth and Retention


## 📄 Project Overview

This project is an in-depth analysis of Waze’s user behavior data, with the goal of identifying key drivers of user churn. By understanding what influences users to stop using the app, I developed actionable strategies to reduce churn and improve user retention. This project demonstrates my expertise in data cleaning, exploratory data analysis (EDA), A/B testing, and generating strategic recommendations based on data-driven insights.

## 🎯 Objectives

The main goals of this analysis are to:

1. **Examine User Behavior**: Use EDA to uncover key behavioral patterns associated with user retention and churn.
2. **A/B Testing for Device Insights**: Perform hypothesis testing to determine if device type impacts user engagement.
3. **Data-Driven Recommendations**: Based on the findings, propose targeted strategies for increasing user retention and enhancing engagement.

## 🛠 Tools and Techniques

- **Programming Language**: Python
- **Environment**: Jupyter Notebook
- **Libraries Used**: `pandas`, `numpy`, `seaborn`, `matplotlib` for data manipulation and visualization; `scipy.stats` for statistical analysis
- **Statistical Testing**: Conducted t-tests to evaluate differences in user behavior by device type
- **Data Cleaning**: Addressed missing values, outliers, and ensured data was prepared for analysis

## 📊 Data Dictionary

The dataset provides various metrics related to Waze user activity, device types, and engagement patterns, including:

| Field                    | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| **label**                | Target variable ("retained" vs. "churned") indicating if a user churned     |
| **sessions**             | Number of app openings by the user in the month                             |
| **drives**               | Number of drives (≥1 km) completed by the user during the month             |
| **device**               | Type of device used (e.g., iPhone, Android)                                 |
| **total_sessions**       | Estimated total app sessions since user onboarding                          |
| **n_days_after_onboarding** | Number of days since user signed up                                    |
| **total_navigations_fav1**   | Total navigations to the user’s favorite place 1 since onboarding     |
| **total_navigations_fav2**   | Total navigations to the user’s favorite place 2 since onboarding     |
| **driven_km_drives**     | Total kilometers driven during the month                                    |
| **duration_minutes_drives**  | Total driving duration in minutes for the month                       |
| **activity_days**        | Days the app was opened in the month                                        |
| **driving_days**         | Days with ≥1 km driven during the month                                     |

**Dataset link** [**here**]()

## 🔍 Key Insights

### Dataset Overview

- **Retention Rate**: 82% of users were retained, while 18% churned.
- **Data Quality**: The dataset had missing values in the `label` column and outliers in key metrics like `driven_km_drives` and `activity_days`.

### User Behavior Insights

1. **Usage Patterns**: 
   - Churned users completed about three more drives in the last month compared to retained users, but retained users opened the app on twice as many days.
   - Churned users drove longer distances and durations per session than retained users.

2. **Engagement Trends**:
   - **App Activity**: Users with higher app activity (sessions) were less likely to churn. Notably, 40% of users who didn’t use the app last month churned, while those who used it daily did not churn.
   - **Driving Frequency**: Users with frequent driving days were more likely to stay retained.

3. **Device Analysis through A/B Testing**:
   - iPhone users demonstrated a slightly higher number of drives on average compared to Android users, though the t-test showed no statistically significant difference in drive frequency between device types.

### Data Distributions

- Many variables were either **right-skewed** (e.g., `total_sessions`, `activity_days`) or **uniformly distributed** (e.g., `n_days_after_onboarding`).
- The skewed distributions indicate most users had lower values in these metrics, with a small number of highly engaged users at the upper end.

## ✅ Recommendations

Based on these findings, I recommend the following strategies for Waze to improve user retention and engagement:

### 1. **Engagement Programs for High-Activity Users at Risk of Churn**
   - Use notifications or rewards targeted toward high-activity users who may still be at risk of churning, which can help keep these valuable users engaged.

### 2. **Segmented Retention Strategies**
   - Analyze user segments within the churned group for common characteristics to design targeted retention strategies.

### 3. **App Interface Enhancements**
   - To improve engagement, consider app usability enhancements for users who are less active, potentially addressing pain points that contribute to churn.

### 4. **Addressing Data Quality**
   - Resolve missing values in key columns and address outliers in driving metrics to ensure data reliability for future analyses.

### 5. **Continued A/B Testing**
   - Continue monitoring user behavior by device type through ongoing A/B testing, as trends may evolve over time.

## 🔮 Next Steps

To build on this analysis, future work could include:

1. **User Segmentation**: Group users by behavior to create more personalized engagement strategies.
2. **Retention Prediction**: Use churn indicators identified here to develop models that predict churn early.
3. **Time-Series Analysis**: Explore changes in user behavior over time to pinpoint trends and proactive retention opportunities.

## 📌 Conclusion

This project provides a thorough analysis of user retention factors within Waze, along with actionable recommendations for improving user satisfaction and reducing churn. The insights presented here serve as a data-driven framework for Waze to strengthen its user base and foster long-term growth.

[**👉 Click Here to View the Full Jupyter Notebook Analysis**](https://github.com/jimi121/PYTHON-PROJECTS/blob/main/Waze%20App%20Users%20Churn%20Analysis/Waze%20App%20analysis.ipynb) <!-- Replace with actual URL -->
