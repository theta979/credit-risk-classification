# credit-risk-classification
Module 20 Challenge
Initial push for module 20 Challenge consisting of starter files and resources.

# Module 20 Report Template

## Overview of the Analysis

This analysis was essentially meant to predict the credit risk of loans based on various factors associated with each loan. The data used to make these predicitons included the Loan size, interest rate, borrowers income, debt to income ratio, nubmer of accounts the borrower has, derogatory marks and total debt.

Once we read the data in from the CSV file, we accomplish this prediction by separating the data, removing the values associated with the "y" or output we are seeking to predict. Splitting the data using the "train_test_split" module from sklearn. I used the StandardScaler to flatten the disance between the values to make the data easier to work with. 

Next, I ceated the Logistic Regression model by fitting the scaled data and training the model on it. Lastly, we created a Confusion matrix to visualize the perfomance of my classfication model and a classification report with the results displayed accessing the Precision, Recall and F1-SCore values.

## Results

- Non-High Risk Loans (0)
-- Precision: 1.00
-- Recall: 0.99
-- f1 Score: 1.00

- High Risk Loans (1)
-- Precision: 0.84
-- Recall: 0.99
-- f1 Score: .91

## Summary

The one point from this model that stands out is it's Precision score for the (1) High Risk loan classification. In this category it's Precision was 84 percent. This indicates that there were some accounts (16%) that the model predicted as High Risk that were not actually hy risk. This could be problematic when it effects an organizations ability to make quality decisions based on the model.