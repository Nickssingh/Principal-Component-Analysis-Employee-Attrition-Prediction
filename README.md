# Principal Component Analysis - IBM Employee Attrition

## A. Goal
Principal Component Analysis (PCA) is used to reduce the number of features needed to be used in a prediction model. In this exercise, we will see the impact of PCA – in terms of accuracy and time needed to train – on models: Logistic Regression, Decision Tree, K Nearest Neighbors, Naive Bayes, and SVM.

## B. Data Source
https://www.ibm.com/communities/analytics/watson-analytics-blog/hr-employee-attrition/

## C. Summary
_Dataset Description_

‘Attrition’ (binary) is the target variable, which we will try to predict. We have 34 input variables – overall including factors such as demographics, travel, education, income, field, and number of years at the current company and role, and with current manager. The features have only 2 datatypes: integers and factors; however, it is important to note that many numerical variables (such as ‘DistanceFromHome’) are ordinal.

_Data Cleaning_

- We did not have any missing values within the dataset.
- We mapped the yes/no in the target variable – Attrition – to 1/0.
- We dropped the ‘EmployeeNumber’ as it does not have any impact.
- Further, after looking at the distribution of the numerical variables, we observed that ‘EmployeeCount’ and ‘StandardHours’ are constants; hence, we will drop these columns as well.

_Exploratory Data Analysis_

1. We can observe that ‘Attrition = 1’ is just 1/6th of ‘Attrition=0’; only 16% of the entire dataset is ‘0’. Thus, this is an unbalanced dataset. However, as we are focusing majorly on understanding the impact of PCA, we will not focus on methods needed to deal with unbalanced data (we have already discussed in one of the other repositories (https://github.com/Nickssingh/SMOTE-Unbalanced-Data-Bank Marketing/blob/master/Bank%20Marketing-Call%20Response%20Prediction.Rmd) how SMOTE can be used to deal with imbalance in data).
2. It appears that among the employees who discontinued, frequent travel is comparatively a larger portion of the group.
