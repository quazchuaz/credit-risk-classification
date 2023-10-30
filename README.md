# Credit Risk Analysis Report

## Overview of the Analysis

* The analysis was conducted in order to determine the creditworthiness of potential customers. Supervised learning models were used to this end.

* Lending information was used to inform the model in question. Loan Status (Healthy or High Risk) constituted the target variable predicted, whilst the features used were loan size, interest rate, borrower income, debt to income ratio, number of accounts, derogatory remarks made and total debt.
 
* It should be noted that the Original Data contained 75,036 counts of healthy loans and only 2,500 counts of high-risk loans.

* The general process of the analysis consisted of first splitting the data into training and testing sets, creating a logistic regression model, training the model on our training set, making predictions using our testing set, and finally evaluating the model's accuracy / explanatory power.

* We applied the above process to a Logistic Regression model using the Original Data in addition to using Resampled data to address the imbalance in counts of healthy and high-risk loans in our dataset.

## Results
* Machine Learning Model 1 - Logistic Regression with Original Data:
•	Balanced Accuracy = 95.20 %

•	Accuracy = 99%

•	Precision (Healthy Loans) = 100%

•	Recall (Healthy Loans) = 99% 

•	Precision (High Risk Loans) = 85%

•	Recall (High Risk Loans) = 91%


* Machine Learning Model 2 - Logistic Regression with Resampled Data:
•	Balanced Accuracy = 99.37%

•	Accuracy = 99%

•	Precision (Healthy Loans) = 100%

•	Recall (Healthy Loans) = 99% 

•	Precision (High Risk Loans) = 84%

•	Recall (High Risk Loans) = 99%

## Summary

* Both Models have strong explanatory power as described by the scores outlined above. Due to the imbalance of counts between healthy and high-risk loans in the dataset Model 2 seems to perform marginally better overall. The precision score for high-risk loans is only 1% lower however there is a significant gain of 8% in the recall score for this type of loan. This means that the risk of false negatives is lower, which in our case translates to the risk of extending credit by mistake to someone who actually has a high risk of default.
  
* It should be noted that evaluating the performance of the model does depend on the specific problem that the model is trying to solve. Depending on this, the relative importance of accurately predicting healthy against high risk loans becomes important. The 1% lower precision value for high-risk loans may matter more if the risk of false positives is more important. In this case a false positive would be the risk of misclassifying a creditworthy customer as one who has high default risk, thereby reducing sales.
In the end, the performance of the model is dependent on the specific question that is being asked of it.
