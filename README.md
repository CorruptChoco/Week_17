# Week_17
## Overview of the analysis
We are using a credit card credit dataset to evaluate credit risk. We balance the samples using two separate oversampling techniques, undersample and combinatorial approach of over- and undersampling. Then we compared two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results
Random Oversampling
* Accuracy: 63.4%

SMOTE Oversampling
* Accuracy: 64.7%

Undersampling
* Accuracy: 54.2%

Combination SMOTEENN
* Accuracy: 65.5%

Balanced Random Forest
* Accuracy: 90.5%

Easy Ensemble AdaBoost Classifier
* Accuracy: 93.7%


* Our highest Accuracy was gained from the Easy Ensemble AdaBoost Classifier.
* Our highest Recall and Precision were also gained from the Easy Ensemble AdaBoost Classifier.


## Summary
If you want the lowest risk to the company you would want a model that has high recall/sensitivity. This way you have the highest potential of identifying all those with a high credit risk. Therefore from our testing we would select the Easy Ensemble AdaBoost Classifier with it's sensitivity of 91% for high risk clients. However, it only has a precision of 7%, meaning that only 7% of the time that when it predicts someone as high risk are they actually high risk. That is a lot of lost revenue on clients that you think are high risk but are actually low risk. For these reasons I can't recommend any of these algorithms for detecting high or low risk for a client.