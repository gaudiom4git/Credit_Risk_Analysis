# Credit_Risk_Analysis

## Overview - Loan Prediction Analysis

This module explained how machine learning can assist with analyzing credit card risk.  Students used Pandas and dataframes to perform data preparation, 
statiscal reasoning and machine learning practices to predict credit card risk.  

Identify target (credit risk outcome)
Identify features (attributes used in machine learning method)
Split the data - training and testing
Train the model (fit)
Make predictions
classification report


## Results 

Results TBD
There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models (15 pt)

### Naive Random Oversampling

![Naive Random Oversampling](https://github.com/gaudiom4git/Credit_Risk_Analysis/blob/main/Resources/NaiveRandomOversampling.png)

* Balance Accuracy Score = 65.16%.  False Negative = 33.
* The precision of prediction using this model:Low Risk(1) is 1 and High Risk(0) is 0.01 
* The recall(sensitivity) for predicting Low Risk(1)is 0.68 and High Risk is 0.62 
* The F1 score for Low Risk is 0.81 and for high risk is 0.02 as precision for High risk is low.

### SMOTE Oversampling

![SMOTE Oversampling](https://github.com/gaudiom4git/Credit_Risk_Analysis/blob/main/Resources/SmoteOversampling.png)

* Balance Accuracy Score = 62.42%.  False Negative = 36.
actually those are High risk. 
* The precision of prediction using this model:Low Risk(1) is 1 and High Risk(0) is 0.01 
* The recall(sensitivity) for predicting Low Risk is 0.59 and High Risk is 0.66 
* The F1 score for Low Risk is higher 0.80

### Undersampling

![Undersampling](https://github.com/gaudiom4git/Credit_Risk_Analysis/blob/main/Resources/Undersampling.png)

* Balance Accuracy Score = 52.75%.  False Negative = 35.  
but actually those are High risk. 
* The precision of prediction using this model:Low Risk(1) is 1 and High Risk(0) is 0.01 
* The recall(sensitivity) for predicting Low Risk is 0.46 and High Risk is 0.60 
* The F1 score for low Risk is higher 0.63 and high risk is 0.01

### Combination (Over and Under) Sampling-SMOTEENN algorithm to Predict Credit Risk

![Combination Over and Under SMOTEEN](https://github.com/gaudiom4git/Credit_Risk_Analysis/blob/main/Resources/SMOTEEN.png)

* Balance Accuracy Score = 52.75%. False Negative = 26.
* The precision of prediction using this model:Low Risk(1) is 1 and High Risk(0) is 0.01 
* The recall(sensitivity) for predicting Low Risk is 0.58 and High Risk is 0.70
* The F1 score for Low Risk is higher 0.73 and high risk is 0.02

### Balanced Random Forest Classifier

![Balanced Random Forest](https://github.com/gaudiom4git/Credit_Risk_Analysis/blob/main/Resources/BalancedRandomForestClassifier.png)

* Balance Accuracy Score = 77.91%. False Negative = 30. 
* The precision of prediction using this model:Low Risk(1) is 1 and High Risk(0) is 0.03 
* The recall(sensitivity) for predicting Low Risk is 0.88 and High Risk is 0.67 
* The F1 score for Low Risk is higher 0.94 and high Risk is 0.06

### Easy Ensemble AdaBoost Classifier

![Easy Ensemble AdaBoost](https://github.com/gaudiom4git/Credit_Risk_Analysis/blob/main/Resources/EasyEnsembleADABoost.png)

* Balance Accuracy Score = 50.00% The False Negative = 0 .  All other models suggest these are not reliable numbers.
* The precision of prediction using this model:High Risk(1) is 1 and Low Risk(0) is 0.00.
* The recall(sensitivity) for predicting Low Risk is 0.00 and High Risk is 1.00 
* The F1 score for Low Risk is higher 0.00 and high risk is 0.01

## Summary

Model with the highest accuracy is Balanced Random Forest at 77.91%   False Negative score was 30 which is low which indicates that 
the model predicted 30 cases where the model predicted a negative credit card risk that was actually positive.
