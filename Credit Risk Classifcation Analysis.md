# Module 20 Report

## Overview of the Analysis

In the credit risk classification analysis, the challenge was to use the Logistic Regression Model as is and also to use the RandomOverSampling module (oversampling the minority data which is the high risk loan status) to make calculations as to the best method to predict if a loan is high risk.  This analysis uses the following algorithms both with and without the RandomOverSampling module to determine which method I would use to make predictions if a borrower is creditworthy provided the data features and entries remain consistent into the future:
- K-Nearest Neighbors Algorithm (kNN)
- Naive Bayes Algorithm
- Logistic Regression Algorithm
- Support Vector Machines (SVM) Algorithm

The purpose for this analysis is to predict if a loan is high risk or "healthy". A "healthy" loan is one where we do not expect the borrower to default. A high risk loan is where the lender assumes risk in that the loan may not get paid. High risk loans tend to have a higher interest rate (to help recoupe costs in the event of a default). The lender depends on the borrower's financial capacity and trust that the loan will be repaid.

The financial information used was a dataset that contained the amount of the loan, the interest rate, borrower's income, debt to income ratio, number of accounts open at the time the loan was made, negative remarks on the borrower's credit history, total debt from their credit history at the time the loan was made, and the loan status (0 is a "healthy" loan and 1 is a high risk loan). We are using various algorithms to make predictions for the likelihood that a loan will be high risk.

The variables used in the prediction is the dependant variable (y) loan status and the independant variables (x) are the loan size, interest rate, borrower's income, borrower's debt to income ratio, number of accounts open, negative remarks on their credit history, and total debt at time of loan.

In the machine learning process we read in the dataset from a csv file and split it into training and test data. We defined the x and y values and scaled those values to prevent skewed calculations. We then created the models listed above for both the original dataset and a random oversampled dataset. This was the training phase to make predictions. Finally, we evaluate the model's performance by creating reports and analyzing the results.
## Results

* K-Nearest Neighbors (kNN) Model 
    - Parameters: n_neighbors = 1, no oversampling

      ![](https://github.com/mugsiemx/credit-risk-classification/blob/main/Credit_Risk/Images/kNN%20nn%201%20ros%20false.png)


* K-Nearest Neighbors (kNN) Model 
    - Parameters: n_neighbors = 1, with oversampling

      ![](https://github.com/mugsiemx/credit-risk-classification/blob/main/Credit_Risk/Images/kNN%20nn%201%20ros%20true.png)


* K-Nearest Neighbors (kNN) Model 
    - Parameters: n_neighbors = 5, no oversampling

      ![](https://github.com/mugsiemx/credit-risk-classification/blob/main/Credit_Risk/Images/kNN%20nn%205%20ros%20false.png)


* K-Nearest Neighbors (kNN) Model 
    - Parameters: n_neighbors = 5, with oversampling

      ![](https://github.com/mugsiemx/credit-risk-classification/blob/main/Credit_Risk/Images/kNN%20nn%205%20ros%20true.png)


*  Naive Bayes Model 
    - Parameters: no oversampling

      ![](https://github.com/mugsiemx/credit-risk-classification/blob/main/Credit_Risk/Images/naive%20bayes%20ros%20false.png)


*  Naive Bayes Model 
    - Parameters: with oversampling

      ![](https://github.com/mugsiemx/credit-risk-classification/blob/main/Credit_Risk/Images/naive%20bayes%20ros%20true.png)


*  Logistic Regression Model 
    - Parameters: no oversampling

      ![](https://github.com/mugsiemx/credit-risk-classification/blob/main/Credit_Risk/Images/lr%20ros%20false.png)


*  Logistic Regression Model 
    - Parameters: with oversampling

      ![](https://github.com/mugsiemx/credit-risk-classification/blob/main/Credit_Risk/Images/lr%20ros%20true.png)


*  Support Vector Machines (SVM) Model 
    - Parameters: no oversampling

      ![](https://github.com/mugsiemx/credit-risk-classification/blob/main/Credit_Risk/Images/svm%20ros%20false.png)


*  Support Vector Machines (SVM) Model 
    - Parameters: with oversampling

      ![](https://github.com/mugsiemx/credit-risk-classification/blob/main/Credit_Risk/Images/svm%20ros%20true.png)


## Summary

The results for the original assignment led us down the path that either the logistic regression model with or without the random oversampling worked out the same. Our main goal is to predict both healthy and high risk loans. All of the models used predict healthy loans with 99% to 100% accuracy. High risk loans have a higher variance where a strong recall score (prediction if a loan is high risk) is high or the precision is high. Ideally we want to see both scores high. We find in these models where K-Nearest Neighbors Algorithm (kNN), Naive Bayes Algorithm, Logistic Regression Algorithm, and Support Vector Machines (SVM) Algorithm with or without random sampling support the businesses goals of predicting loans accurately with strong predictions regarding precision, recall, and the f1-score. We would recommend any of these models except the K-Nearest Neighbors with 1 nearest neighbor with or without oversampling. While the precision is high at 98%, predicting if a loan is high risk (recall at 86%) is low.
