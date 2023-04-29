# Report

## Overview of the Analysis

This analysis was created to leverage an existing dataset in order to predict the creditworthiness of borrowers. The predictions are sorted as either 'high-risk loans' or 'healthy loans'. The financial information included in the data are: loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, total debt, and loan status. Loan status was used as the label against the other features. The information in the inital Logistic Regression model was unbalanced, with 75,000 variables for healthy loans and only 2,500 for high-risk. It became balanced in the random over sampler model with around 56,000 variables for each class. For each model, the machine learning process was the same. The data was read, split, fit, and the model ran predictions before running a confusion matrix, balanced accuracy, and classification report. 

## Results

* Machine Learning Model 1: Logistic Regression
  * accuracy: 0.9442676901753825

   *  precision -- recall -- f1-score -- support
 
Healthy:     1.00  ---  1.00 --- 1.00 --- 18759

High-Risk:   0.87 -- 0.89 -- 0.88 -- 625





* Machine Learning Model 2: Random Over Sampler
  * accuracy: 0.9959744975744975

  * precision -- recall -- f1-score -- support

Healthy:       1.00  ---  1.00  ---  1.00  ---  18759

High-Risk:       0.87 -- 1.00 -- 0.93 -- 625

## Summary

The results of both models would inspire confidence in the predictions. Based on the high accuracy, precision, and recall of both models, either would be a good choice for performance, but the Random Over Sampler model is slightly better. I know it is more accurate because the confusion matrix showed less errors than the original logistic regression model. So I would recommend the balanced Random Over Sampler model for prediction use.
