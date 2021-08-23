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
#### SMOTE Oversampling

### Undersampling
#### Cluster Centroids

### Combination (Over and Under) Sampling
#### SMOTEENN


 
## Summary
### Results Summary
As summary of the results in presented in the table below

As demonstrated in the analysis above the balanced accuracy score ranges between 60-90%. The first four models have an accuracy score in the 60s. For the last two models the score is relatively higher. The balanced accuracy sore in not a good indictor when dealing with imbalanced classes, such as is the case here.
The models using yield a low precision score. This indicates that the financial institutions have a high percentage of false positives when it comes to high risk scores. 
  


### Recommendation



