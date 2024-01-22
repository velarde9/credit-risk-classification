# Module 12 Credit Risk Classification: Risk Analysis Report 


## Overview of the Analysis

## Purpose
The purpose of this analysis is to analyze the performance of the machine learning models used in this challenge. These models are compared against each other to determine which model is better at evaluating loan risk and identifying the creditworthiness of borrowers and to predict the loan status of these borrowers, between healthy loans and high-risk laons.

## Dataset
The dataset contains historical lending activity from a peer-to-peer lending services company such as loan size, interest rate,	borrower income, debt to income, number of accounts, derogatory marks, total debt, and loan status. Overall, out of 77,536 borrowers, there were 75,036 healthy loans, and 2500 high-risk loans.

## Method
The starter code notebook was used to read the lending_data.csv data from the Resources folder into a Pandas DataFrame. From here, the labels set (y) was created from the "loan_status" column and the features (X) dataframe was created with the remaining columns. The data was then split into training and testing datasets using train_test_split.

The training and testing data were fit into a logistic regression model with random_state = 1. Two predictions were made, where the second prediction resampled the data using RandomOverSampler. The new prediction data was then fit into another logistic regression model and results in the classification reports were compared to the first model.


## Results

* Machine Learning Model 1:
  * Balanced accuracy score: 95%
  * Accuracy score: 99%
  * Healthy Loans Precision score: 100%
  * Healthy Loans Recall score: 100%
  * High-Risk Loans Precision score: 86%
  * High-Risk Loans Recall score: 90%

* Machine Learning Model 2:
  * Balanced accuracy score: 99%
  * Accuracy score: 99%
  * Healthy Loans Precision score: 100%
  * Healthy Loans Recall score: 99%
  * High-Risk Loans Precision score: 84%
  * High-Risk Loans Recall score: 99%


## Summary

The first model had an accuracy score of 99% percent, meaning that it was able to predict 99% of positive cases correctly. For healthy loans, precision and recall scores were 100%. For High-rish loans, the precision score was 86% and the recall score was 90%.

For the second model, the accuracy score was also 99%. For healthy loans, the presicion score was 100% and the recall score was 99%. For High-rish loans, the precision score was 84% abd the recall score was 99%. 

The balanced accuracy score for the second model was 99%, whereas the balanced accuracy score for the first model was only 95%. 

For this example, it would be better to use the second model as it has a higher balanced accuracy score, and was able to better predict high-risk loans. When determining the creditworthiness of borrowers, it is more important for the model to accurately predict high-risk loans as the number of high-risk loans will influence the overall creditworthiness of borrowers more than the number of health loans would.
