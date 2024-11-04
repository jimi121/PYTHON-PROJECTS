# Employee Retention Analysis Project



## 📊 Project Overview

In today’s competitive business landscape, retaining skilled employees is essential for organizational success. High employee turnover can incur substantial costs and negatively impact productivity and morale. Recognizing the critical nature of this issue, this project dives into a comprehensive HR dataset to uncover patterns and trends driving employee turnover. By leveraging data analytics and predictive modeling, this project aims to deliver actionable insights, enabling organizations to proactively address the root causes of employee attrition.

## ⚙️ Project Objective

The primary goal of this project is to analyze the HR dataset to build a predictive model that identifies employees at risk of leaving. Through advanced analytics techniques, this project provides a predictive tool for organizations to enhance employee retention, foster engagement, and support strategic HR decision-making.

### Significance

This project can fundamentally transform how organizations approach employee retention. By systematically examining HR data, it provides actionable insights to guide strategic decisions, allowing organizations to:
- Reduce recruitment and training costs associated with turnover.
- Develop targeted initiatives to address root causes of employee attrition.
- Foster a more positive, engaged, and stable work environment.

---

## 🛠️ Tools and Technologies

This project was developed using Python and Jupyter Notebook, leveraging:
- **Data Processing**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Predictive Modeling**: Scikit-learn (Logistic Regression)

---

## 📝 Data Dictionary

The dataset contains 14,999 records and 10 variables:

| Variable                 | Description                                                                                |
|--------------------------|--------------------------------------------------------------------------------------------|
| `satisfaction_level`     | Employee's self-reported job satisfaction level (0–1)                                      |
| `last_evaluation`        | Score of the employee's last performance review (0–1)                                      |
| `number_project`         | Number of projects the employee contributes to                                             |
| `average_monthly_hours`  | Average hours worked per month by the employee                                             |
| `time_spend_company`     | Years the employee has been with the company                                               |
| `Work_accident`          | Whether or not the employee experienced an accident at work                                |
| `left`                   | Indicator if the employee left the company                                                 |
| `promotion_last_5years`  | Indicator if the employee was promoted in the last 5 years                                 |
| `Department`             | The employee's department                                                                  |
| `salary`                 | Employee's salary level (categorized)                                                      |

**Dataset link** [**here**]()

---

## 🔍 Key Findings

1. **Burnout and Overwork**: Employees with lower satisfaction levels, longer working hours, and multiple projects are more likely to leave, suggesting burnout as a critical factor.
2. **Tenure and Loyalty**: Employees who have been with the company for over six years show higher retention, indicating a loyalty trend among longer-tenured employees.
3. **Impact of Promotions and Recognition**: Employees with recent promotions or high evaluation scores exhibit greater satisfaction, suggesting that professional growth and recognition are pivotal retention drivers.

The logistic regression model used in this analysis achieved:
- **Precision**: 79%
- **Recall**: 82%
- **F1-Score**: 80%
- **Accuracy**: 82%

These metrics underscore the model's reliability in predicting turnover and identifying at-risk employees.

---

## ✅ Recommendations

To reduce turnover, the following actionable steps are recommended:

1. **Limit Project Overload**: Cap the number of projects assigned to each employee to prevent burnout.
2. **Promotion Strategy**: Consider promoting employees who have been with the company for at least four years or investigate potential dissatisfaction factors.
3. **Reward or Adjust Working Hours**: Either compensate employees for longer hours or reassess the need for excessive overtime.
4. **Transparent Policies**: Clearly communicate overtime and workload expectations.
5. **Company-Wide Culture Assessment**: Foster discussions on workplace culture and identify areas of improvement across teams and departments.
6. **Evaluation Criteria**: Re-evaluate the criteria for performance reviews to ensure that they fairly reward effort without exclusively favoring long hours.

---

## 📌 Conclusion

Implementing these recommendations can help improve employee retention by creating a healthier, more supportive work environment that values balance and recognizes contributions. Embracing these insights will ultimately cultivate a resilient and engaged workforce, contributing to the organization’s long-term success.

---

## 🚀 Next Steps

Future work could involve:
- Implementing other machine learning models (e.g., Random Forest, Gradient Boosting) to improve prediction accuracy.
- Examining additional data (e.g., employee engagement survey results) to enrich analysis and model accuracy.

---

[**👉 Click Here to View the Full Jupyter Notebook Analysis**](https://github.com/jimi121/PYTHON-PROJECTS/blob/main/Employee%20retention%20prediction%20project/Employee%20retention%20prediction.ipynb) <!-- Replace with actual URL -->

