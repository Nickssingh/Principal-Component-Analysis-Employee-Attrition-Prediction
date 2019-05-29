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
