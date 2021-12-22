# AlmaBetter Capstone Project 3 - Classification : Credit-Card-Default-Prediction
This project is a part of the **AlmaBetter Premium Program** , Banglore/Bengaluru ,Karnataka , India

Project Status: **[Completed]**

![1_uZyt9Z189siaNsAlIDtjEg](https://user-images.githubusercontent.com/88345564/147155410-6462b88e-ebf4-4558-98d6-75d9bc6c7d06.jpeg)


### Problem Description :
This project is aimed at predicting the case of customers default payments in Taiwan. From the perspective of risk management, the result of predictive accuracy of the estimated probability of default will be more valuable than the binary result of classification - credible or not credible clients. We can use the K-S chart to evaluate which customers will default on their credit card payments.

### What is credit card default?
Credit card default happens when you have become severely delinquent on your credit card payments. Default is a serious credit card status that affects not only your standing with that credit card issuer but also your credit standing in general and your ability to get approved for other credit-based services.

### How Credit Card Default Happens?
When you accept a credit card, you agree to certain terms. For example, you agree to make your minimum payment by the due date listed on your credit card statement. If you miss the minimum payment six months in a row, your credit card will be in default. Your credit card issuer will likely close your account and report the default to the credit bureaus.

### Approach Taken
* Data inspection and cleaning
* Exploring data, checking for outliers
* Clean data to get it ready for Analysis
* EDA & Data Pre-processing

-- Checking distributions of variable

-- Univariate and multivariate analysis

-- Checking for imbalanced dataset. We have used **SMOTE** here.

* Modelling (Implementing Machine Learning Algorithms)
1. Logistic
2. KNN
3. Decision Tree + Random Forest
4. XGBoost
5. SVM

* Model Evaluation
* Conclusions

### Models Used

**Logistic Regression Classifier Algorithm**

LR Classifier Generator 

LR Hyper Parameter Tuning : GridSearch

Final Logistic Regression Training run

**K Nearest Neighbours Classifier Algorithm**

Default Parameters : KNeighborsClassifier

KNN Model Generator Funciton

KNN Hyper Parameter Tuning : GridSearch

Final KNN Training run

**Random Forrests of Decsision Trees**

Default Parameters : RandomForestClassifier

Base Estimator Generator Function

HyperParameter tuning using GridSearchCV

Final Training Run

**Gradient Boosted Trees using XGBoost Library**

XGBoost algorithn training and tuning notes

XGBoost Estimator Instance Generator Function

HyperParameter tuning using BayesSearchCV

Final Training Run for XGBoost

Feature Importance

**SVM(support vector machine)**

Default Parameters : SvmClassifier

SVM Model Generator Funciton

SVM Hyper Parameter Tuning : GridSearch

Final SVM Training run


## **Conclusions**

We investigated the data, checking for data unbalancing, visualizing the features, and understanding the relationship between different features. We then investigated two predictive models. The data was split into three parts, a train set, a validation set, and a test set. For the first three models, we only used the train and test set.


We started with Logistic Classifier and then with RandomForrestClassifier, knn model,SVM.


We then experimented with an XGBoost model. In this case, we used the validation set for validation of the training model. The best validation score obtained was 0.912. Then we used the model with the best training step to predict the target value from the test data; the AUC score obtained was 0.910 which is less then the validation score of random forest .random forest perform best in this problem data set with higest recall more then 86% and precision is also high for random forest and highest AUC score of around 0.912.so over all Random forest is the winner from the all the remaining model.


Random Forest is the best model for card card default prediciton with an accuracy of 83%.
