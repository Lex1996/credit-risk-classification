# Credit Analysis Report

## Purpose of the Analysis:

The purpose of this analysis is to develop and evaluate machine learning models for credit risk classification. The goal is to predict whether a loan is high-risk (label 1) or not (label 0) based on various financial features.

## Financial Information and Prediction Target:

The data used in this analysis contains information about loans, including features such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The prediction target is the "loan_status" column, where 0 represents a healthy loan and 1 represents a high-risk loan.

## Basic Information about Variables:

The dataset consists of 75,036 healthy loans (label 0) and 2,500 high-risk loans (label 1).
The features used for prediction include numerical variables related to loan characteristics.
Stages of the Machine Learning Process:

* Data Preprocessing: The data is loaded, and features (X) and labels (y) are separated. The dataset is then split into training and testing sets.

* Model 1: Logistic Regression with Original Data:

    * A logistic regression model is trained using the original training data.
    * Predictions are made on the testing data.
    * Model performance is evaluated using accuracy, a confusion matrix, and a classification report.

* Model 2: Logistic Regression with Resampled Data:

    * Data is resampled using the RandomOverSampler to balance the labels.
    * A logistic regression model is trained using the resampled data.
    * Predictions are made on the resampled data.
    * Model performance is evaluated using accuracy, a confusion matrix, and a classification report.

## Methods Used:

Logistic Regression: Used for both models to perform binary classification.

## Results

* Machine Learning Model 1:

    * Balanced Accuracy Score: 95.20%
    * Precision for label 0: 100%
    * Precision for label 1: 84.61%
    * Recall for label 0: 99.45%
    * Recall for label 1: 90.79%

* Machine Learning Model 2 (Logistic Regression with Resampled Data):

    * Balanced Accuracy Score: 99.45%
    * Precision for label 0: 99.47%
    * Precision for label 1: 99.47%
    * Recall for label 0: 99.47%
    * Recall for label 1: 99.47%

## Summary:

* Model 2 (Logistic Regression with Resampled Data) outperforms Model 1 (Logistic Regression with Original Data) in terms of balanced accuracy, precision, and recall.
* Model 2 exhibits exceptional performance with near 99% accuracy and near-perfect precision and recall for both label 0 and label 1.
* The choice of the model may depend on the problem's specific requirements. Model 2 is recommended for scenarios where accurate prediction of both healthy and high-risk loans is crucial.

In summary, the logistic regression model trained with resampled data performs exceptionally well in predicting credit risk, making it the preferred choice for this classification task. The performance of the models suggests that it is possible to accurately classify high-risk loans based on the provided financial features.