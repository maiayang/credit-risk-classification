# credit-risk-classification

## Overview

In this challenge, we analyzed lending data to create a logistical regression model to predict loan status (0: Healthy loan, 1: High-risk loan). Factors such as loan size, interest rate, borrower income, and debt-to-income ratio were used for the predictions. The original dataset contained 75,036 loans classified as healthy and 2,500 loans classified as high-risk.

First, the columns were separated into features (X) and labels (y). Then the data was split into training and testing data for both X and y. Next an instance of a Logistic Regression model was created using the LogisticRegression module from SKLearn. Finally, the model was fit to the training data and predictions were made using the testing data.

## Results

The precision and recall scores for the "0" (Healthy) loans are perfect due to a large sample size. In actuality, when looking at the confusion matrix, 80 healthy loans were misclassified as high-risk, and 67 high-risk loans were misclassified as healthy.

The precision and recall scores for the "1" (High-risk) loans are slightly worse than the "0" (Healthy) loans with a precision score of .87 and recall score of .89. 


## Summary

Based on the results, the model is considered to be very good in predicting credit worthiness. It is advantageous for banks to have a better precision/recall for predicting "High-Risk" loans versus "Healthy" loans. However since there are less high-risk loans than healthy loans, this must be taken into consideration as well when analyzing the scores from a statistical standpoint. 

In this scenario, it is better to have a higher recall rate than precision rate for the "high-risk" loans. The reason for this is that banks would rather incorrectly classify a loan as "high-risk" when it is actually "healthy", as opposed to incorrectly classifying a loan as "healthy" when it is actually "high-risk". This model has a higher recall rate (.89) than precision rate (.87) for the "high-risk" loans so I would recommend this model for predicting credit-worthiness.