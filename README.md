## Credit Risk Classification Analysis Report
# Module 20

## Table of Contents
- Overview of the Analysis
- Results
- Summary

## Overview of the Analysis
The objective of this analysis was to develop a model for assessing the creditworthiness of borrowers based on historical lending data. The dataset included various financial attributes of borrowers, and the goal was to predict whether a loan is classified as high-risk or healthy.

## The analysis involved the following steps:

- Splitting the data into training and testing sets.
- Creating a logistic regression model using the original data.
- Predicting loan status using a logistic regression model trained on resampled training data.
- Writing a credit risk analysis report.

A logistic regression model was selected as the machine learning algorithm, and resampling techniques were employed to address the imbalanced nature of the data.

## Results

# Machine Learning Model 1: Logistic Regression Model (Original Data)
- Balanced Accuracy Score: 95.2%
- Precision and Recall:
   - Healthy Loans (Label 0):
     - Precision: 100%
     - Recall: 99%
   - High-Risk Loans (Label 1):
     - Precision: 85%
     - Recall: 91%

The model achieved a high balanced accuracy score; however, it performed poorly in predicting high-risk loans (label 1), with only 85% precision. This indicates the model was more effective at predicting healthy loans (label 0) than identifying high-risk loans.

## Machine Learning Model 2: Logistic Regression Model (Oversampled Data)
- Balanced Accuracy Score: 99.4%
- Precision and Recall:
   - Healthy Loans (Label 0):
     - Precision: 100%
     - Recall: 99%
   - High-Risk Loans (Label 1):
     - Precision: 99%
     - Recall: 99%

The logistic regression model trained on oversampled data showed improved results compared to the original data model. The balanced accuracy score increased to 99.4%, and the precision for high-risk loans rose to 99%, indicating a significant improvement in identifying high-risk loans.

## Summary
The logistic regression model trained on oversampled data (Machine Learning Model 2) outperformed the original data model. It demonstrated higher precision and recall for high-risk loans, which is crucial for identifying potential credit risks.

For assessing loan risk, it is essential to have high precision for high-risk loans (label 1) to minimize the chances of misclassifying loans with higher default probabilities. Machine Learning Model 2 showed a significant improvement in this regard.

Therefore, it is recommended to use Machine Learning Model 2 for credit risk assessment, as it provides better performance in identifying high-risk loans and offers more accurate predictions for creditworthiness analysis.