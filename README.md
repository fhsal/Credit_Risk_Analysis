# Credit Risk Analysis

CWRU Data Analytics Module Seventeen Challenge


## Overview of Project

The project involved using supervised machine learning models with a credit risk dataset containing information regarding consumer home loan credit histories and loans being sought to purchase homes.  The data included information such as income, current rent/own status, assessment of loan risk, loan amounts and interest rates, etc.     
  

## Analysis 

The Challenge focused upon building six machine learning models using the consistent approach of pre-processing the dataset using the getdummies() method to convert relevant string variables into numeric 0/1 values for modeling purposes, resampling the data, splitting into trainging/target, train the model, determine accuracy score, create a confusion matrix and generate a classification report.  The six models are:


Four LogisticRegression models:  

* after resampling using RandomOverSampler

* after resampling using SMOTE

* after resampling using ClusterCentroids

* after over/under resampling using SMOTEEN 

Two ensemble classifier models:

* using BalancedRandomForestClassifier

* using EasyEnsembleClassifier


### Summary

The ensemble models generally perform better than logistic Regression, with boosting producing better results than bagging.   This is likely due to the underlying data distribution and variance where multiple iterations outperform single iteration modeling.  The Logistic Regression models range in balanced accuracy from .51 to .65 whereas the Ensemble models range from .78 to .92.  I did, however, notice that my results are somewhat different from those in the sample file - which may be due to how I used getdummies(), but our TA indicated the basic results were in line with expectations.  

### Model Results  

Based upon the balanced accuracy scores, either of the Ensemble models could be used.   The Logisitic Regression models are relatively poor predictors. 

## Linear Regressions

**RandomOverSampler**

![img](https://github.com/fhsal/Credit_Risk_Analysis/tree/main/main/RandomOverSampler.png)

**SMOTE**

![img](https://github.com/fhsal/Credit_Risk_Analysis/tree/main/main/RandomOverSampler.png)


**ClusterCentroids**  

![img](https://github.com/fhsal/Credit_Risk_Analysis/tree/main/main/RandomOverSampler.png)

**SMOTEEN**  

![img](https://github.com/fhsal/Credit_Risk_Analysis/tree/main/main/RandomOverSampler.png)


## Ensemble Models

**BalancedRandomForestClassifier**

![img](https://github.com/fhsal/Credit_Risk_Analysis/tree/main/main/BalancedRandomForestClassifier.png)

**EasyEnsembleClassifier**

![img](https://github.com/fhsal/Credit_Risk_Analysis/tree/main/main/EasyEnsembleClassifier.png)