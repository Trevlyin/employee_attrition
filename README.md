# IBM HR: Employee Attrition Analysis
## by Trevlyin M.I Muzinda

![attrition](High-employee-turnover.jpg)

## Dataset

The HR Employee Attrition dataset is a fictional dataset consisting of 1470 employees, pulled together by IBM specialists and made available through the [data.world](https://data.world/aaizemberg/hr-employee-attrition) platform. It contains information on employees demographic and other situational standings with attrition status.
Some of the ordinal categorical variables in the dataset represents a rating attained from the same author via [Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)

For more information on what is employee attrition, check out [this blog](https://traqq.com/blog/employee-attrition-vs-employee-turnover-whats-the-difference/)

## Summary of Findings

Among 1470 employees, about 16% was affected by attrition and in turn, this became the attrition rate. After sourcing out the rate the next step was to discover possible factors on why employees leave the company. Firstly we found out group attrition rates for all categorical data and among them, the only employee demographic that stood out was Marital Status, where Single employees are affected by 25.53% compared to the rest of the attrition sample. There was a surprising trend in the attrition rate in accordance with the Work-Life Balance  of employees where one would expect a negative correlation from Bad to Best ratings but got an unusual spike on Best rating making it the second high attrition rate after Bad rating of this group. This outcome commanded further investigation hence after pairing it with other features like `EnvironmentSatisfaction` there was a similar distribution but when the employees were very satisfied with their work environment. `OverTime` and `BusinessTravel` was also included as part of the investigation. 

After isolating the selected sample to not include those with low environment satisfaction, overtime workers and those who travel frequently for work, it resulted in the negative correlation with the work-life balance sample for employees who were part of the attrition.

Since the numerical variables did not yield any significant relationship with `Attrition`, I found a relationship between `Age` and `TotalWorkingYears` where it also highlighted the company's age diversity as they were employees above 38 years of age upto 60 years who had little to no experience.

## Key Insights for Presentation

For the presentation I would be focusing on the categorical variables that had high risk in their groups which include `MaritalStatus`, `JobInvolvement`,`EnvironmentSatisfaction`,`OverTime`, `BusinessTravel`, and `WorkLifeBalance`. I will start by introducing the attrition distribution with a countplot and the attained attrition rate.

Secondly, will look at the categorical variable influences on attrition one by one. Since it is category to categorical mapping for each visual I will be using seaborn's barplots and finally regarding my suggestions for decreasing attrition rate in the company will use a stacked bar chart. The color palette used is to distinguish the group with a high attrition risk and for the last suggestion visual is to highlight the decrease in attrition rate.
