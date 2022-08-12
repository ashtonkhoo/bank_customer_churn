![Banner](https://miro.medium.com/max/640/1*RAeucVCKyFGXArObBsYnrw.png)

# Table of contents

- [Project Title](#project-title)
- [Project Description](#project-description)
- [Project Workflow](#project-workflow)
- [Dataset](#dataset)

# Project Title
Bank Customer Churn Analysis & Prediction with XGBoost

# Project Description
This project aims to analyze the bank-customers-churn dataset available on Kaggle, and perform some predictive analysis on whether a given customer will exit or not.

# Project Workflow
- Load the dataset into a pandas dataframe.
- Perform exploratory data analysis, identifying presence of null & duplicated values, as well as some preliminary statistics about the data.
- Calculate the correlation matrix to identify correlated features, if any.
- Encode categorical features to numerical values, as the selected algorithm (XGBoost) cannot handle categorical values by itself.
- Check distribution of label classes. Discovered that labels were imbalanced, and used ADASYN to oversample the minority class.
- Split the dataset into training and testing sets with a 70/30 split.
- The XGBoost classifier is then trained on the training set, with initial parameters, and is used to make predictions on the test set. The predictions are compared and evaluated with the actual test set labels to calculate the accuracy and root mean squared error (RMSE).
- Apply hyperparameter tuning using Random Search on some candidate parameter grid, with a 5-fold cross-validation for 100 iterations.

# Dataset 
Santosh Kumar. 2018. "Bank Customers Churn", version 1. Retrieved 11/08/2022 from https://www.kaggle.com/datasets/santoshd3/bank-customers.
