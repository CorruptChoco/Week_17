# Week_17
## Overview of the analysis
We are using a credit card credit dataset to evaluate credit risk. We balance the samples using two separate oversampling techniques, undersample and combinatorial approach of over- and undersampling. Then we compared two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results
Random Oversampling
![Naive_Random_Oversampling](https://user-images.githubusercontent.com/96025706/165422606-9f6d0c34-1837-4d68-820d-bf06fe441743.png)
* Accuracy: 63.4%

SMOTE Oversampling
![SMOTE_Oversampling](https://user-images.githubusercontent.com/96025706/165422621-02f2fa54-f435-4cc3-85c4-1acfd1032d0b.png)
* Accuracy: 64.7%

Undersampling
![Undersampling](https://user-images.githubusercontent.com/96025706/165422633-bf122b2a-b4ab-4b18-84b1-b0991e782684.png)
* Accuracy: 54.2%

Combination SMOTEENN
![Combination_Sampling](https://user-images.githubusercontent.com/96025706/165422676-84855082-8cd8-4a85-a529-3a679b161d84.png)
* Accuracy: 65.5%

Balanced Random Forest
![Balanced_Random_Forest](https://user-images.githubusercontent.com/96025706/165422692-0cbef61c-ac0a-4e9e-ae46-27a03dc9facc.png)
* Accuracy: 90.5%

Easy Ensemble AdaBoost Classifier
![Adaboost](https://user-images.githubusercontent.com/96025706/165422712-9da0bc62-8cdc-4b04-a4ff-d70f0a4dd42f.png)
* Accuracy: 93.7%


* Our highest Accuracy was gained from the Easy Ensemble AdaBoost Classifier.
* Our highest Recall and Precision were also gained from the Easy Ensemble AdaBoost Classifier.

## Summary
If you want the lowest risk to the company you would want a model that has high recall/sensitivity. This way you have the highest potential of identifying all those with a high credit risk. Therefore from our testing we would select the Easy Ensemble AdaBoost Classifier with it's sensitivity of 91% for high risk clients. However, it only has a precision of 7%, meaning that only 7% of the time that when it predicts someone as high risk are they actually high risk. That is a lot of lost revenue on clients that you think are high risk but are actually low risk. For these reasons I can't recommend any of these algorithms for detecting high or low risk for a client.
