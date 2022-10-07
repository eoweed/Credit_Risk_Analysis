# Credit_Risk_Analysis
Use Machine Learning to Predict Credit Card Risk

## Overview:
#### The purpose of this project is to create and compare six supervised machine learning models that will predict credit card risk with the classification of low-risk or high-risk loan status. The dataset used to train and test the models is provided by the LendingClub and contains information about loans and credit card data. The goal is to determine which model can most accurately predict loan status.
#### Loan and credit card data usually contain unbalanced classifications for the target variable. In other words, when analyzing and predicting loan status there are usually many more good loans than bad loans. The six machine learning models that will be used contain sampling strategies that will balance out the data before making predictions.
1. RandomOverSampler
2. SMOTE
3. ClusterCentroids
4. SMOTEENN
5. BalancedRandomForestClassifier
6. EasyEnsembleClassifier

## Results:
###### Below are the evaluations of each machine learning model showing the accuracy of the model, and the precision and sensitivity of predicting high-risk and low-risk loan status. 

#### ---------------------------------------------------------------
<img src="https://github.com/eoweed/Credit_Risk_Analysis/blob/main/images/Resampling-Models-Evaluation.png">

#### ---------------------------------------------------------------
<img src="https://github.com/eoweed/Credit_Risk_Analysis/blob/main/images/BalancedRandomForestClassifier.png">

#### ---------------------------------------------------------------
<img src="https://github.com/eoweed/Credit_Risk_Analysis/blob/main/images/EasyEnsembleClassifier.png">

#### ---------------------------------------------------------------

###### RandomOverSampler:
-	Accuracy: 0.661
-	Precision (High-Risk): 0.01
-	Precision (Low-Risk): 1.00
-	Sensitivity (High-Risk): 0.72
-	Sensitivity (Low-Risk): 0.60

###### SMOTE:
-	Accuracy: 0.658
-	Precision (High-Risk): 0.01
-	Precision (Low-Risk): 1.00
-	Sensitivity (High-Risk): 0.62
-	Sensitivity (Low-Risk): 0.69

###### ClusterCentroids:
-	Accuracy: 0.545
-	Precision (High-Risk): 0.01
-	Precision (Low-Risk): 1.00
-	Sensitivity (High-Risk): 0.69
-	Sensitivity (Low-Risk): 0.40

###### SMOTEENN:
-	Accuracy: 0.653
-	Precision (High-Risk): 0.01
-	Precision (Low-Risk): 1.00
-	Sensitivity (High-Risk): 0.74
-	Sensitivity (Low-Risk): 0.56

###### BalancedRandomForestClassifier:
-	Accuracy: 0.789
-	Precision (High-Risk): 0.03
-	Precision (Low-Risk): 1.00
-	Sensitivity (High-Risk): 0.70
-	Sensitivity (Low-Risk): 0.87

###### EasyEnsembleClassifier:
-	Accuracy: 0.932
-	Precision (High-Risk): 0.09
-	Precision (Low-Risk): 1.00
-	Sensitivity (High-Risk): 0.92
-	Sensitivity (Low-Risk): 0.94


## Summary:
#### Accuracy:
###### Most of the models were not very accurate, however the EasyEnsembleClassifier model was the most accurate with a 93.2% chance of correctly predicting loan status. 
#### Precision:
###### The precision of predicting high-risk was very low for every model, while the precision of predicting low-risk was 100% for every model.
#### Sensitivity:
###### The sensitivity scores were moderate for each of the models, however the EasyEnsembleClassifier model had the highest sensitivity score for predicting both high-risk and low-risk loan status with both scores above 90%.
#### Best Performing Model:
###### Overall, the best model out of the six that were evaluated, is the EasyEnsembleClassifier model. When predicting loan status, it is important to use a model with high sensitivity for predicting high-risk loans so that loaners can be aware of all loans that may be high-risk, even if some of them may be falsely predicted with that status. 