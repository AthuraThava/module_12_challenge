# Module_12_Challenge: Credit Risk Analysis Report
![image](https://github.com/AthuraThava/module_12_challenge/assets/125240804/f1a686c2-19b4-412a-86c6-976ba1feb9a4)

## Overview of Analysis

The purpose of this anlysis is to identify the creditworthiness of borrowers, by uilizing a dataset of historical lending activity from a peer-to-peer lending services company to build a Logistic Regression Model for original and minulated data.This analysis aims to predict Confusion Matrix, Accuracy, Precision and Recall score for two models.
The stages of the machine learning process that were taken during this analysis are:

* Split the Data into Training and Testing Sets
* Create a Logistic Regression Model with the Original Data
* Predict a Logistic Regression Model with Resampled Training Data
* Write a Credit Risk Analysis Report

## Results

Machine Learning Model 1: Logistic Regression Model with the Original Data

* Accuracy:0.9520479254722232

![image](https://github.com/AthuraThava/module_12_challenge/assets/125240804/14044efc-b186-4d1a-96e2-30dc6772d136)

Machine Learning Model 2: Logistic Regression Model with Resampled Training Data

* Accuracy:0.9936781215845847

![image](https://github.com/AthuraThava/module_12_challenge/assets/125240804/b458664e-4af1-4b15-b5b0-623574b6e0ee)

## Summary

The logistic regression model with original data predicts a precision of 1.00, recall of 0.99, and specificity of 0.91, which demonstrates its high accuracy in predicting the "0" (healthy loan) label. The model performs well for the "1" (high-risk loans), but not quite as well as "0" (healthy loans). The precision is 0.85, recall is 0.91, and specificity is 0.99 for this method. Overall, the model performs sufficiently in terms of both healthy and high-risk loans, with healthy loans doing better in terms of accuracy.

Since the dataset is unbalanced and the number of healthy loans ("0") outweighs the number of high-risk loans ("1"), the findings may be deceptive since the model would be more inclined to predict a healthy loan. As a result, it is crucial to forecast the model using resampled data.

The 0 (healthy loan) and 1 (high-risk loan) are both accurately predicted by the logistic regression model fitted using oversampled data. A balanced accuracy score of 99% was produced by the oversampled model, which is greater than the model using the original (imbalanced) data. With a small decline in recall for the high-risk loan class compared to the original model, the model has good accuracy and recall for both loan types.

The logistic regression model 2 with oversampled data is the recommend model to use, since the model better represents high risk loans. Since the original intent of this analysis is to accurate identify high risk loans, as healthy loans easily outnumber risky loans.
