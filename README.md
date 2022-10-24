# Capstone-Project-Credit-Card-Fraud-Detection-

The Credit Card Fraud detection Data:

https://www.kaggle.com/kartik2112/fraud-detection?select=fraudTest.csv

https://www.kaggle.com/kartik2112/fraud-detection?select=fraudTrain.csv

The challenge is to recognize fraudulent credit card transactions so that the customers of credit card companies are not charged for items that they did not purchase.
Data is collected for the period of 01/01/2019-12/31/2020.There are 23 columns in the data and 1852394 rows of transaction records. The column ‘is_fraud’ can be considered as the entire data label/target, which will be predicting.

All columns:

trans_date_trans_time - Transaction Date/Transaction Time
cc_num - Customer's Credit Card Number
merchant - Merchant by whom the trade occured
category - Type of Purchase
amt - Amount of Transaction
first - First Name
last - Last Name
gender - Customer's Gender
street - Street Address
city - Home City
state - State
zip - Zip Code
lat - Latitude of the Customer
long - Longitude of the Customer
city_pop - Population of the City
job - Customers Jop Title
dob - Customer's Date of Birth
trans_num - Unique Transaction Number for Each Transaction
nix_time - Time of the Transaction in Unix
merch_lat - Merchant Latitude
merch_long - Merchant Longitude
is_fraud - The Fraudulent Transaction /Not


The Fraud case in the entire Data is imbalanced , therefore it is essential to balance the data and  make sure that the classes are nearly equal to each other in order to work with ML algorithms.


Non-fraudulent transactions-99.48%
Fraudulent transactions-0.52%

Takeaway Key:


Extreme Gradient Boosting (XGBoost) is an open-source library that provides an efficient and effective implementation of the gradient boosting algorithm. ... XGBoost can be used directly for regression predictive modeling. In this tutorial, you will discover how to develop and evaluate XGBoost regression models in Python.

Using AUC - ROC curve is a performance measurement for the classification problems at various threshold settings. ROC is a probability curve and AUC represents the degree or measure of separability. It tells how much the model is capable of distinguishing between classes. Higher the AUC, the better the model is at predicting 0 classes as 0 and 1 classes as 1. By analogy, the Higher the AUC, the better the model is at distinguishing between transactions fraudulent or not.
The ROC curve is plotted with TPR against the FPR where TPR is on the y-axis and FPR is on the x-axis.

Precision quantifies the number of positive class predictions that actually belong to the positive class. Recall quantifies the number of positive class predictions made out of all positive examples in the dataset. F-Measure provides a single score that balances both the concerns of precision and recall in one number.



 CONCLUSION
 
I've investigated the data, checked for imbalance, visualized the features and understood the relationship between different features.
The data was split into 2 parts train and test sets . Four different Supervised Machine
Learning algorithmshavebeenused:LogisticRegression,DecisionTreeClassifier,RandomForest Classifier and XGBoost Classifier as well as two techniques for imbalanced
data TheRandomUndersampledtechniqueand SMOTEtechnique. TheGridSearchwasused to find optimal hyper parameters of Random Forest and XGBoost models . As a result of modeling , bestscoreperformedRandomForestwith OptimizedHyperparameterswithUnderSample technique.
Future Work.
One additional work that could have been achieved but could not be completed due to time crunch was using neural networks to see if it could further improve the model results. Also, if I could have time for each of the models, I would apply other techniques for imbalanced data and tune my models.

Copyright Iuri Catasov   
