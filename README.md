# credit-risk-classification
In this Challenge, various techniques wass used to train and evaluate a model based on loan risk. A dataset of historical lending activity from a peer-to-peer lending services company was used to build a model that can identify the creditworthiness of borrowers.

The instructions for this Challenge are divided into the following subsections:
- Split the Data into Training and Testing Sets
- Create a Logistic Regression Model with the Original Data
- Write a Credit Risk Analysis Report

# Split the Data into Training and Testing Sets
The starter code notebook was used to complete the following steps:
- Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.
- Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.
- Split the data into training and testing datasets by using train_test_split.

# Create a Logistic Regression Model with the Original Data
A Logistic regression model was created using the following steps:
- Fit a logistic regression model by using the training data (X_train and y_train).
- Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.
- Evaluate the model’s performance by doing the following:
- Generate a confusion matrix.
- Print the classification report.

# Write a Credit Risk Analysis Report
A brief report was written, which includes a summary and analysis of the performance of the machine learning models that was used in this challenge.
This report contains the following:
- An overview of the analysis: Explain the purpose of this analysis.
- The results: Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.
- A summary: Summarize the results from the machine learning model. Include the justification for recommending the model for use by the company. 