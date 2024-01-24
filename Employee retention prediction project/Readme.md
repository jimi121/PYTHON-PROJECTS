# Employee retention project¶

### Introduction:

In today's competitive business landscape, retaining skilled and talented employees is paramount for the sustained success of any organization. Employee turnover not only incurs substantial financial costs but also poses a threat to the overall productivity and morale within the workplace. Recognizing the significance of this issue, our project delves into the analysis of a comprehensive HR dataset to discern patterns and trends that may elucidate the factors influencing employee departure. By harnessing the power of data analytics and predictive modeling, we aim to provide actionable insights that can empower organizations to proactively address issues contributing to employee turnover.

### Objective:

The primary objective of this project is to leverage the HR dataset to develop a robust predictive model capable of anticipating whether an employee is likely to leave the company. By employing advanced analytics techniques, we aim to identify key indicators and patterns within the data that correlate with employee turnover. Additionally, our goal is to unravel the complex interplay of various factors, ranging from job satisfaction and work-life balance to professional growth opportunities, which contribute to the decision of employees to seek alternative employment. Ultimately, the project seeks to equip organizations with a predictive tool that aids in mitigating employee turnover and fostering a more stable and engaged workforce.

### Significance:

The significance of this project lies in its potential to revolutionize how organizations approach employee retention. By systematically analyzing the wealth of data collected by HR departments, we aim to provide actionable insights that can guide strategic decision-making. The ability to predict employee turnover allows for proactive interventions, enabling companies to implement targeted initiatives addressing the root causes identified in the analysis. This, in turn, not only saves substantial costs associated with recruitment and training but also contributes to a more positive and stable work environment. As businesses strive to attract and retain top talent, our project's findings can serve as a valuable resource for HR professionals and organizational leaders seeking to enhance employee satisfaction, well-being, and overall retention rates.

## Data Dictionary

In this [dataset](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction?select=HR_comma_sep.csv), there are 14,999 rows, 10 columns, and these variables: 

Variable  |Description |
-----|-----| 
satisfaction_level|Employee-reported job satisfaction level [0&ndash;1]|
last_evaluation|Score of employee's last performance review [0&ndash;1]|
number_project|Number of projects employee contributes to|
average_monthly_hours|Average number of hours employee worked per month|
time_spend_company|How long the employee has been with the company (years)
Work_accident|Whether or not the employee experienced an accident while at work
left|Whether or not the employee left the company
promotion_last_5years|Whether or not the employee was promoted in the last 5 years
Department|The employee's department
salary|The employee's salary (U.S. dollars)

[Click here to see analysis in the notebook](https://github.com/jimi121/PYTHON-PROJECTS/blob/main/Employee%20retention%20prediction%20project/Employee%20retention%20prediction.ipynb)

# Insight from the Dataset
It appears that employees are leaving the company as a result of poor management. Leaving is tied to longer working hours, many projects, and generally lower satisfaction levels. It can be ungratifying to work long hours and not receive promotions or good evaluation scores. There's a sizeable group of employees at this company who are probably burned out. It also appears that if an employee has spent more than six years at the company, they tend not to leave.

The classification report shows that the logistic regression model achieved a precision of 79%, recall of 82%, f1-score of 80% (all weighted averages), and accuracy of 82%.

# Recommendations

To retain employees, the following recommendations could be presented to the stakeholders:

* Cap the number of projects that employees can work on.
* Consider promoting employees who have been with the company for atleast four years, or conduct further investigation about why four-year tenured employees are so dissatisfied. 
* Either reward employees for working longer hours, or don't require them to do so. 
* If employees aren't familiar with the company's overtime pay policies, inform them about this. If the expectations around workload and time off aren't explicit, make them clear. 
* Hold company-wide and within-team discussions to understand and address the company work culture, across the board and in specific contexts. 
* High evaluation scores should not be reserved for employees who work 200+ hours per month. Consider a proportionate scale for rewarding employees who contribute more/put in more effort. 

# Conclusions

In conclusion, the implementation of these recommendations is poised to not only enhance employee retention but also contribute to the establishment of a workplace that values its workforce, promotes a healthy work-life balance, and fosters a positive and supportive culture. As stakeholders move forward, embracing these insights can lead to a more resilient, engaged, and satisfied employee base, ultimately contributing to the long-term success of the organization.
