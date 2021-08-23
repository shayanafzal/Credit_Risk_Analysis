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
### Results Summary




Oversampling 
1.	Naive Random Oversampling
*   Accuracy Score: 66.69%
*   Precision
    * High Risk: 0.01
    * Low Risk: 1.00
*   Recall
    *	High Risk: 0.67
    *	Low Risk: 0.6

2.	SMOTE Oversampling
*	 Accuracy Score: 62.69%
*	 Precision
    *	 High Risk: 0.01
    *	 Low Risk: 1.00
*	 Recall
    *	 High Risk: 0.57
    *	 Low Risk: 0.68

3. Cluster Centroids
*	Accuracy Score: 62.69%
*	Precision
   *	High Risk: 0.01
   *	Low Risk: 1.00
*	Recall
   *	High Risk: 0.57
   *	Low Risk: 0.68

4. Combination of Over and Under Sampling
*	Accuracy Score: 65.02%
*	Precision
   *	High Risk: 0.01
   *	Low Risk: 1.00
*	Recall
   *	High Risk: 0.72
   *	Low Risk: 0.58

5. Balanced Random Forest Classifier
*	Accuracy Score: 79.58%
*	Precision
   *	High Risk: 0.03
   *	Low Risk: 1.00
*	Recall
   *	High Risk: 0.71
   *	Low Risk: 0.88

6. Easy Ensemble AdaBoost Classifier
*	Accuracy Score: 92.64%
*	Precision
   *	High Risk: 0.08
   *	Low Risk: 1.00
*	Recall
   *	High Risk: 0.91
   *	Low Risk: 0.94






As summary of the results in presented in the table below

As demonstrated in the analysis above the balanced accuracy score ranges between 60-90%. The first four models have an accuracy score in the 60s. For the last two models the score is relatively higher. The balanced accuracy sore in not a good indictor when dealing with imbalanced classes, such as is the case here.
The models using yield a low precision score. This indicates that the financial institutions have a high percentage of false positives when it comes to high risk scores. 
  


### Recommendation



