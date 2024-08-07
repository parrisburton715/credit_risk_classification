# Machine Learning Model Analysis for Loan Status Prediction

## Overview of the Analysis
Purpose of the Analysis
The goal of this analysis was to build and evaluate a machine learning model to predict loan status based on a dataset of financial information. Specifically, the objective was to classify loans into different statuses, such as default or non-default.

Financial Information and Prediction Goal
The dataset used (lending_data.csv) that contains information related to loans, including financial and personal details of borrowers. The target variable, loan_status, indicates whether a loan is in default. My task was to predict this loan status using the features provided in the dataset.

Basic Information About the Variables
Target Variable (loan_status): This variable indicates the status of the loan. The value_counts would show how many loans fall into each category, e.g., 0 for non-default and 1 for default.
Features (X): These features include various financial and personal attributes of borrowers used to predict the loan status.
Stages of the Machine Learning Process
Data Preparation: The data was loaded into a Pandas DataFrame and inspected. The target variable (loan_status) was separated from the features.
Train-Test Split: The data was split into training and testing sets using train_test_split, with a random seed set for reproducibility.
Model Selection: A Logistic Regression model was chosen for classification.
Model Training: The Logistic Regression model was trained using the training data.
Model Evaluation: Predictions were made on the test data, and the model's performance was evaluated using a confusion matrix and classification report.
Methods Used
Logistic Regression: A statistical model used for binary classification tasks. It predicts the probability of a categorical dependent variable based on one or more predictor variables.

## Results
*Machine Learning Model 1: Logistic Regression

Accuracy: 0.99

The model correctly predicted 99% of the instances in the test set.


*Precision:

For class 0 (non-default): 1.00

For class 1 (default): 0.85

Precision indicates the proportion of true positive predictions out of all positive predictions made.


*Recall:

For class 0 (non-default): 0.99

For class 1 (default): 0.91

Recall measures the proportion of actual positives that were correctly identified by the model.

## Summary
Model Performance
Best Performing Model: The Logistic Regression model performs very well with an overall accuracy of 99%. It achieves high precision and recall for class 0, and reasonable performance for class 1.
Performance Considerations: Although the model performs well overall, the precision and recall scores for class 1 (default) are lower compared to class 0 (non-default). This indicates that while the model is very effective at predicting non-default loans, it is slightly less effective at identifying default loans.
Recommendation
The Logistic Regression model seems to be the most effective model in this analysis, given its high accuracy and balanced performance metrics. However, for financial applications, it might be more critical to improve recall for the default class (1), as failing to identify a default loan could have significant consequences.
The procision for class 1 is not optimal but it will do.
