# Credit-Risk-Analysis

## Overview of Analysis

This analysis will focus on utilizing machine learning to build models to predict credit risk for loans. In addition, we will utilize these models to a evaluate the performance and see how well they predict data.

### Results

The data preparation utilizes Machine Learning and Pandas to analyze and create models. The summaries are generated on the <a href="credit_risk_resampling.ipynb">Credit Risk Resampling file</a> and <a href="credit_risk_ensemble.ipynb">Credit Risk Ensemble file</a>. 

In this analysis, we utilize 6 machine learning tests:

- Oversampling Alogrithms: RandomOverSampler and SMOTE
- Undersampling Algorithm: ClusterCentroids
- Combination Approach Algorithm of Over and Undersampling: SMOTEENN
- Reduce Bias Algorithms: BalancedRandomForestClassifier and EasyEnsembleClassifier

### RandomOverSampler Model

After conducting the RandomOverSampler algorithm, the results of the test is that the balanced accuracy score is 64%. In addition, the high_risk precision is 1% with a 66% sensitivity result. As a result, the low_risk population is almost 100% with a sensitivity result of 62%.

### SMOTE Model

After conducting the SMOTE algorithm, the results of the test is that the balanced accuracy score is 65%. The high_risk precision is 1% with a 61% sensitivity result. Whereas, the low_risk population is almost 100% with a sensitivity result of 69%.

The results of the SMOTE Model is similar to the RandomOverSampler Model.

### ClusterCentroids Model

After conducting the ClusterCentroids algorithm, the results of the test is that the balanced accuracy score is 54%. The high_risk precision is 1% with a 69% sensitivity result. Therefore, the low_risk population is 100% with a sensitivity result of 40%.

### SMOTEENN Model

After conducting the SMOTEENN algorithm, the results of the test is that the balanced accuracy score is 64%. The high_risk precision is 1% with a 71% sensitivity result. As a result, the low_risk population is 100% with a sensitivity result of 57%.

### BalancedRandomForestClassifier Model

After conducting the BalancedRandomForestClassifier algorithm, the results of the test is that the balanced accuracy score is 79%. The high_risk precision is 3% with a 70% sensitivity result. Therefore, the low_risk population is 100% with a sensitivity result of 87%.

### EasyEnsembleClassifier Model

After conducting the EasyEnsembleClassifier algorithm, the results of the test is that the balanced accuracy score is 93%. The high_risk precision is 9% with a 92% sensitivity result. Whereas, the low_risk population is 100% with a sensitivity result of 94%.

## Summary

After creating 6 different models and testing the performance of each, all the models used to perform the credit risk analysis show weak precision in determining if a credit risk is high. For example, the EasyEnsembleClassifier Model is a strongner model in comparison to the others, specially on the sensitivity of the high risk credits. This is demonstrated with its 92% high_risk precision so it detects almost all high risk credit. However, with a low precision, a lot of low risk credits are still falsely detected as high risk. This can alter and jeopordize the bank's credit strategy. 

As a result, I would not recommend the bank to use any of these models to predict credit risk. 