# credit-risk-classification

## Overview of the Analysis
The data was analyized using models created by machine learning algorithims. The source dataset consisted of lending historical data, which contained the necessary information to create the risk-analysis data model to determine lending to borrowers.

The dataset included: loan amount, interest rate, borrower income, debt to income, number of accounts, derogatory marks, total debt and loan status. 

The purpose of the data model that was created is to predict if the loan is a "healthy loan" or "high-risk loan." 

The data model was two dimentional that had a y variable, which contained the "loan_status", and a x variable, which contained the features. After, the x and y variables were set the value_counts function was used to check the balance.

Using the established variables the data was then fit into two datasets-training and testing. Based on the nature of the dataset a logical regression model was used for training and testing the model.

Resources used for the evaluation of the model were "confusion_matrix", "balanced_accuracy_score", and "classification_report."

## Results
* Machine Learning Model 1:
Accuracy: 0.9442676901753825 • Precision: 0 (healthy loan) 1.00; 1 (high-risk loan) 0.87 • Recall: 0 (healthy loan) 1.00; 1 (high-risk loan) 0.89
* Machine Learning Model 2:
Accuracy: 0.9959744975744975 • Precision: 0 (healthy loan) 0.99; 1 (high-risk loan) 1.00 • Recall: 0 (healthy loan) 0.87; 1 (high-risk loan) 1.00


## Summary
The regression model resulted in an accuracy of 0.9442676901753825 showing a high level of validity. There were 19,237 correct predictions and only 147 false predictions for "healthy loans." The models precision accuracy for "high-risk loans" is .87 or 87%. The model can more accurately predict "healthy loans" than "high-risk loans". In a real application the percentage of accuracy for "healthy loans" is within an acceptable range. However, addtional data is required for "high-risk loans" to increase the prediction accuracy to an acceptable range.

The oversampled model is able to predict high-risk loans and healthy loans with a high level of precision. Once, the minority class was oversampled the model improves its precision. The recall also increases to 1 for the high-risk loans.

The recommendation to ensure the highest level of accuracy of the risk-analysis would be to oversample the minority class of "high-risk loans" and then a regression model. This would ensure unbias and balance results. 


