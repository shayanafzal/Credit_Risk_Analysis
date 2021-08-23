# Credit Risk Analysis

## Overview of the Loan Prediction Risk Analysis
### Purpose
Good loan easily out number risky loans. Hence, credit risk is an unbalanced classification problem. Therefore, this analysis employs different techniques to train and evaluate models with unbalanced classes and presents are recommendation on whether they should be use to predict credit risk.
### Libraries Used
For the purpose of this analysis ‘imbalanced-learn’ and ‘scikit-learn’ are the two libraries that have been used to build and evaluate models using resampling.
### Method Used
For this analysis credit card credit data was gathered from LearningClub which is a peer-to-peer lending services company. The data was oversampled using ‘RandomOverSampler’ and ‘SMOTE’ algorithms. The data was then undersampled using the ‘ClusterCentroids’ algorithm. Lastly, a combinatorial approach of over and undersampling was employed using the ‘SMOTEENN’ algorithm.

After this the two machine learning models, ‘BalacedRandomForecastClassifier’ and ‘EasyEnsembleClassifier’, that are used to reduce bias to predict credit risk. Lastly, the performance of the aforementioned methods is compared and a recommendation is presented on whether they should be used to predict credit risk.

## Results


### Oversampling 
#### Naive Random Oversampling
![GitHub Logo](https://github.com/shayanafzal/Credit_Risk_Analysis/blob/6c3a8edc51765ccc3237991d1767dd922d2d62ce/Resources/Naive%20Random%20Oversampling.png)
#### SMOTE Oversampling
![GitHub Logo](https://github.com/shayanafzal/Credit_Risk_Analysis/blob/6c3a8edc51765ccc3237991d1767dd922d2d62ce/Resources/SMOTE%20Oversampling.png)

### Undersampling
#### Cluster Centroids
![GitHub Logo](https://github.com/shayanafzal/Credit_Risk_Analysis/blob/6c3a8edc51765ccc3237991d1767dd922d2d62ce/Resources/Undersampling%20ClusterCentroids.png)

### Combination (Over and Under) Sampling
#### SMOTEENN
![GitHub Logo](https://github.com/shayanafzal/Credit_Risk_Analysis/blob/6c3a8edc51765ccc3237991d1767dd922d2d62ce/Resources/Combination%20Smoteenn.png)

### Balanced Random Forest Classifier
![GitHub Logo](https://github.com/shayanafzal/Credit_Risk_Analysis/blob/6c3a8edc51765ccc3237991d1767dd922d2d62ce/Resources/Balanced%20Random%20Forest%20Classifier.png)
### Easy Ensemble AdaBoost Classifier
![GitHub Logo](https://github.com/shayanafzal/Credit_Risk_Analysis/blob/6c3a8edc51765ccc3237991d1767dd922d2d62ce/Resources/Easy%20Ensemble%20AdaBoost%20Classifier.png)

## Summary
### Results Summary & Analysis

A qualitative summary of the results obtained for the six methods has been presented above. As demonstrated in the analysis above the balanced accuracy score ranges between 60-90%. The first four models have an accuracy score in the 60s. For the last two models the score is relatively higher. The balanced accuracy sore in not a good indictor when dealing with imbalanced classes, such as is the case here. The models using yield a low precision score. This indicates that the financial institutions have a high percentage of false positives when it comes to high risk scores. 

All six methods used in this analysis have a precision score of 1. This indicates that all four models return a significant number of false postivies. Looking at the recal sensitivy score for the model used in this analysis, once can see that they are all over 50%. Futhermore, the recal sensitivyt score for the ensemble models is higher than the other methord. This indicates that the ensemble models are more reliable in inidcating low or high risk loans. Lasty looking at the F1 scores one can conclude that there is a high number of false positives and negatives when it comes to high risk loans.  

### Recommendation

Based on the analysis of the six models, it is eveident that the Easy Ensemble AdaBoost Classifier model yield the most accurate results. Based on the limited data we have, Easy Ensemble AdaBoost Classifier would be the recommended model to use.


