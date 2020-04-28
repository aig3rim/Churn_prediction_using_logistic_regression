# Churn_prediction_using_logistic_regression

## Introduction
Customer **churn**, also known as customer attrition, occurs when customers stop doing business with a company. The companies are interested in identifying segments of these customers because the price for acquiring a new customer is usually higher than retaining the old one. For example, if Netflix knew a segment of customers who were at risk of churning they could proactively engage them with special offers instead of simply losing them.

**Logistic Regression** is a Machine Learning classification algorithm that is used to predict the probability of a categorical dependent variable. In logistic regression, the dependent variable is a binary variable that contains data coded as 1 (yes, success, etc.) or 0 (no, failure, etc.). In other words, the logistic regression model predicts P(Y=1) as a function of X.

### Motivation
I was curious to apply logistic regression to predict customer churn.

### Data
In this notebook, a customer churn prediction model is built using Telco Customer Churn <a href=https://www.kaggle.com/blastchar/telco-customer-churn> dataset </a>.


## Getting started
You need an installation of Python, plus the following libraries:

* numpy
* pandas
* matplotlib.pyplot
* seaborn
* sklearn
* imblearn
* statsmodels.api

## Summary and key findings
* This logistic regression model can predict churn with 0.82 accuracy, which can help to retain old users;
* The model gives 1,786 correct and 379 incorrect predictions of churn;
* In order to implement the model, Synthetic Minority Oversampling Technique (SMOT) and Recursive Feature Elimination (RFE) were applied to balance the data and select the important features; 
* After apllying RFE, we chose parameters with p-value less than 0.05. Overall, the model was implemented using the following parameters: "gender_Female", "gender_Male", "SeniorCitizen_No", "SeniorCitizen_Yes", "Dependents_No","MultipleLines_No", "MultipleLines_Yes", "StreamingMovies_No internet service", "Contract_One year", "Contract_Two year", "PaperlessBilling_Yes", "PaymentMethod_Bank transfer (automatic)", "PaymentMethod_Credit card (automatic)", "PaymentMethod_Electronic check", "PaymentMethod_Mailed check".
