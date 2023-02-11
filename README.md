# A classification model to predict whether a customer will ("soon") stop doing business with SyriaTel


![Brazil-Telecommunications-1080x675](https://user-images.githubusercontent.com/117146053/218270842-c37a5b6a-7c5a-4398-aa77-312bdb26bbd5.jpg)

## Overview
This project aims to predict whether a customer will ("soon") stop doing business with SyriaTel using different models. The dataset is obtained from kaggle containing information on features that can give us more information on whether the customer will churn.

## Research Question

Build a classifier model to predict whether a customer will ("soon") stop doing business with SyriaTel.

## Specific Objectives
* To determine which features determine if a customer will churn
 * To increase the recall score to minimize false negatives. 
 
 ## Data Understanding
### Data Source
The dataset used in this project was obtained from Kaggle.
### Data Description
The bigml_59c28831336c6604c800002a.csv contains 3333 rows and 21 columns. The columns cointain both numerical and categorical data.
### Data Preparation
The data was checked to ensure it was in useable form. This was done by checking duplicates, null values and outliers.

## Explanatory Data Analysis
### Count plot of customers who churned and who did not churn
![image](https://user-images.githubusercontent.com/117146053/218281788-0fbe219b-1bec-4453-83e2-c4b6a296c683.png)

### Total Day Charges Distribution
![image](https://user-images.githubusercontent.com/117146053/218281822-186f66a5-e91b-4472-8586-0cf3df88f388.png)

### Relationship between churn and customer service calls
![image](https://user-images.githubusercontent.com/117146053/218281894-92a454df-d70b-483c-859e-84521b3c035c.png)

## Modelling
Baseline model was constructed using logistic regression and the output displayed. 
The baseline model had poor metrics and thus other models were fitted. They included the DesionTree Classifier, K-Nearest Neighbor Classifier and the RandomForest Classifier.
Among the three models, the RandomForest Classifier has the best metrics hence hyperparameter tuning was applied to optmize it. Other more sophisticated models were added to the fray, Gradient Boost Classifier and AdaBoost Classifier.

The Gradient Boost Classifier was the best model overall since it had the highest recall score which was the best at correctly classifying the customers who were soon to discontinue their services with SyriaTel.

## Conclusion
1. The initial goal of achieving 80% accuracy is achieved by all the models that were fitted.
2. Gradient Boost Classifier model provides the highest recall score of all the models.
3. Customer service calls, international plan, total day charges are the features with the greatest importance.

## Repository Guide
The data used for the project can be found here [https://github.com/Mwikali-5/Churn/blob/main/bigml_59c28831336c6604c800002a.csv]

The notebook that contains the project can be found here 

The presentation for this project can be found here [https://github.com/Mwikali-5/Churn/blob/main/Churn.pdf]

A Data Report for this project can be found here [https://github.com/Mwikali-5/Churn/blob/main/Data%20Report_%20Churn.docx]

