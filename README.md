# credit-risk-classification
# Credit Risk Analysis Report

## Overview of the Analysis
In this analysis, I applied my knowledge of supervised machine learning models to a dataset of lending activity from a peer-to-peer lending services company. My goal was to build a model that could identify the creditworthiness of borrowers. 
The dataset I worked with contained several useful features about each borrower, including loan size, interest rate, income, debt to income ratio, number of accounts, derogatory marks, total debt, and loan status. The target column was assigned to the ‘loan status’ column, where each row contained either a 0 or a 1 as the value for this column. This represented the status of the loan, where 0 indicated that the loan was healthy, and 1 indicated that the loan had a high risk of defaulting. 
After assigning my target and feature variables, I used the ‘test_train_split` from the sklearn module to split my data into training and testing datasets. 
Once I had my data split, I used the training data to build my model using ‘LogistsicRegression’ from the sklearn module. I did this by fitting my data to the Logistic Regression classifier. 
Now that my model had seen the training data, I used the Logistic Regression classifier to make predictions on my test data (that my model had not yet seen). 

## Results
Evaluation: 

• Accuracy : 0.99 (99%)

• Precision: 0_healthy : 1.00 (100%) // 1_high_risk :  0.85 (85%)

• Recall : 0_healthy :  0.99 (99%) // 1_high_risk : 0.88 (88%)

## Summary
Overall, I feel that this model’s performance met expectations. I did find it interesting that the accuracy score on the model was 100%, while the precision score of the high-risk loan predictions was only 85%. I believe that because there are so many healthy loans in comparison to the number of high-risk loans. This causes our classes to become imbalanced, leaving more room for false positives. This might explain why our high-risk precision score is a little lower. 

If the goal of this model is to predict the creditworthiness of borrowers, I would want my model to have less room for error. The goal of the lender is to approve borrowers who have a strong likelihood of paying the loan back. I would want to minimize the number of false positives to avoid the risk of lending to unqualified borrowers. 
To do this, I might try a few different methods. I might try a different machine learning model or apply different sklearn libraries to better predict qualified borrowers. 
