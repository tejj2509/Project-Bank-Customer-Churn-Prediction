# Project-Bank-Customer-Churn-Prediction

### Customer Churn Analysis
Customer Churn prediction means to know which customers are likely to unsubscribe or leave the company's services, often since acquiring new customers is more difficult than retaining the existing customer base. In customer churn analysis with the help of a few input data we can predict if the customer is about to leave or exit the service and get in touch with that particular customer and get to know their expectations and try and reach it, thereby retaining the customer. This plays a very significant role in maintaining the business's revenue. In the current scenario, the churn prediction of bank customers is demonstrated.

# About Dataset

This data set contains details of a bank's customers and the target feature is a binary variable reflecting the fact whether the customer left the bank (closed his account) or he continues to be a customer.

Link: https://www.kaggle.com/datasets/shrutimechlearn/churn-modelling


## Features

### RowNumber:

Row Numbers from 1 to 10000.


### CustomerId:

Unique Ids for bank customer identification.


### Surname:

Customer's last name.


### CreditScore:

Credit score of the customer. 


### Geography:

The country to which the customer belongs.


### Gender:

The customer's Gender (Male or Female).

### Age:

Age of the customer.


### Tenure:

Number of years the customer has been with the bank.


### Balance:

Current Bank balance of the customer.


### NumOfProducts:

Number of bank products the customer is utilising.


### HasCrCard:

Whether the customer holds a credit card with the bank or not.


### IsActiveMember:

Whether the customer is an active member with the bank or not.


### EstimatedSalary:

Estimated salary of the customer in Dollars.


### Exited:

1 if the customer closed their account with the bank and 0 if the customer is retained.



The dataset can also be found within this repository.

Data Preprocessing is done by using label encoding, one hot encoding, feature scaling, imbalance data treatment by using Over Sampling technique.

Exploratory Data Analysis (EDA) EDA has been performed to understand the distribution and behaviour of all the input features.

Model Building Logistic Regression for binary classification, Random Forest, Bagging Classifier models are used and to build the final implementable machine learning model Random Forest model is used. The model is having train and test accuracy of 100% and 95% repectively.

Model Evaluation: Model's performance has been evaluated using Clawssification Report, Confusion Matrix, Accuracy score, Recall Score and Cross Validation tests for both test and train datasets.

Usage: The model can be trained as shown in the .ipynb file and relevant input variables can be given to predict the output by using the following example code: prediction = rfc.predict(scaler.transform([[CreditScore, Gender, Age, Tenure, Balance, NumOfProducts, HasCrCard, IsActiveMember,EstimatedSalary, Geography_Germany, Geography_Spain]]))

Outcome:
'The Bank is at high risk of losing this customer'
OR
'The Bank is at a very low risk of losing this customer'
