# Financial-Loan-Eligibility-Analyzer

Real-time Prediction of Loan Approval based on Customer Information

**Table of contents**

Introduction

Project Overview

Data Wrangling

Exploratory Data Analysis

Data Preprocessing

Modeling and Evaluation

Hyperparameter Tuning and Final Model Selection

Conclusion and Next Steps

**Introduction**

This repository contains a comprehensive analysis of a loan eligibility prediction dataset. The project uses several machine learning models to predict whether a loan would be approved or not based on a number of different factors.

**Project Overview**

The dataset consists of a number of variables including loan ID, gender, marital status, employment type, level of education, property area, and loan status (approved/rejected). The main goal of this project is to build an accurate model that can predict whether a loan application would be approved or not.

**Data Wrangling**

The raw data was preprocessed for analysis:

Loaded the data from a CSV file
Explored the dataset's info and description
Handled missing values by replacing them with the mode for categorical variables and with the median for numerical variables
Detected and removed outliers in 'ApplicantIncome', 'CoapplicantIncome' and 'LoanAmount' features

**Exploratory Data Analysis**

An extensive exploratory data analysis was conducted to understand the relationship between different variables:
<img width="1031" alt="Screenshot 2023-06-18 at 9 30 36 AM" src="https://github.com/Abhi0323/Financial-Loan-Eligibility-Analyzer/assets/112967999/e9634945-4aa7-4d42-944e-be9a168b93a5">
<img width="1031" alt="Screenshot 2023-06-18 at 9 30 56 AM" src="https://github.com/Abhi0323/Financial-Loan-Eligibility-Analyzer/assets/112967999/3e56d88b-887e-4616-97ea-4a413e2eba22">

Plotted various graphs and visualizations to understand the distribution of the different variables
Visualized the correlation matrix to see if there are any strongly correlated features
Visualized the count of approved and not approved loans for different categories

**Data Preprocessing**

For the machine learning models to work, some preprocessing steps were required:

Dropped the 'Loan_ID' column, which is a unique identifier and doesn't contribute to the model
Used label encoding to convert categorical values to numeric values
Used log transformation to reduce the skewness of 'ApplicantIncome' and 'CoapplicantIncome'

**Modeling and Evaluation**

Several machine learning models were built and evaluated:

Trained different classifiers (KNeighbors, SVM, DecisionTree, LogisticRegression, NaiveBayes, RandomForest)
Evaluated the performance of these models by calculating their accuracy score

**Hyperparameter Tuning and Final Model Selection**

The Random Forest Classifier was selected as the final model and a grid search was performed for hyperparameter tuning:

Tuned the parameters using GridSearchCV
Generated a detailed classification report and confusion matrix
The final model had an accuracy of around 78%

**Conclusion and Next Steps**

Through this project, I have created a machine learning model that predicts whether a loan would be approved or not with an accuracy of around 78%. The final model can be further improved by exploring more features and trying different modeling techniques.
