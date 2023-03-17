# credit-risk-classification

# Credit Risk Report

## Puporse of the analysis

The purpose of this analysis is to create a model using machine learning so that we can predict whether a loan will be a healthy loan or a high risk loan. By using this model credit broakers will be able to assess whether the loans that they are giving will not be paid back based on the information given.

## What financial information was the data on and what are we trying to predict

This model takes into consideration financial information such as the size of the loan, the interest rate, borrower income, debt to income, number of accounts, derogatory marks and total debt. Using this information we are trying to predict whether we will have a healthy loan [0] or an high risk loan [1].

## Information on predict variable
The data that we were analysing containined information on 75036 healthy loans [0] and 2500 high risk loans [1].

![image](https://user-images.githubusercontent.com/114998403/226019284-84f0dd6e-e970-475f-9f31-2c7794e40405.png)

I then resampled the data so that they both had the same number on samples for healthy and high risk loans to train the model

![image](https://user-images.githubusercontent.com/114998403/226019981-11853438-4449-4ff0-90ed-078e3a1e3de6.png)

## Stages of Machine learning that I went through

Firstly, I created the label variable [y] as the "loan status" and created a variable [X] for the feature which was everything else from the dataframe. I then split the data using the train_test_split method from sklearn using the random_state 1. I then created the logistic regression model and fit it with the training data. I then used this liner regression model to make predictions using the test data. I then calculated the balanced accuarcy score and created the confusion matrix / classification report to get the information ion the perfomance of the model. Using the RandomOverSampler module I then resampled the data so that it had equal number of data points before repeating the process.

## Machine learning Model 1:
* Machine learning model 1 had a balanced accuarcy score of 0.9520479254722232
* Machine learning Model 1 Confusion Matrix and Classification Report:

![image](https://user-images.githubusercontent.com/114998403/226024325-eea8c3d4-f8f9-42bb-84d3-cd3f39939d8c.png)

## Machine learning Model 2
* Machine learning model 2 had a balanced accuracy score of 0.9936781215845847
* Machine learning Model 2 Confusion Matrix and Classification Report:

![image](https://user-images.githubusercontent.com/114998403/226024862-be35903b-93ca-41ad-bee4-0b9d4adf6b78.png)

## Summary

I believe that both of these models performed well at identifying which loans would predict healthy [0] and high risk loans [1]. Model 2 had a better performance than model 1 as it had higher accuracy and higher balnaced accuracy scores. Model 2 also had much less false positive results then compared to model 1. This means that it would clarify much less loans that we deemed healthy however turned out to be risky which would heavily impact the lenders business. Both models are very precise in predicting health loans however struggle abit more in predicting high risk loans. 

Overall, I would choose model 2 to predict whether a loan will be healthy or not.





