# Credit Risk Analysis

## Overview

This project is to build and evaluate different models from imbalanced-learn and scikit-learn libraries for unbalanced classes in data. The credit card credit dataset from LendingClub, a peer-to-peer lending services company is used for this analysis. Models built and evaluated for this project are RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN, BalancedRandomForestClassifier and EasyEnsembleClassifier.

## Results

Different models were evaluated to compare their performance for unbalanced classes dataset. The balanced accuracy, confustion matris and classification report was calculated for each of the models and the results are shown below.

- RandomOverSampler
The balanced accuracy score was 0.65. Precision for high_risk was 0.01 and low_risk was 1.0. Sensitivity was 0.69 and 0.61 for high_risk and low_risk respectively.

![ros](https://github.com/ssathyanath/Credit_Risk_Analysis/blob/main/Images/Random_Oversampling.PNG)

- SMOTE
The balanced accuracy score was 0.66. Precision for high_risk was 0.01 and low_risk was 1.0. Sensitivity was 0.67 and 0.42 for high_risk and low_risk respectively.

![SMOTE](https://github.com/ssathyanath/Credit_Risk_Analysis/blob/main/Images/SMOTE.PNG)

- ClusterCentroids
The balanced accuracy score was 0.54. Precision for high_risk was 0.01 and low_risk was 1.0. Sensitivity was 0.67 and 0.61 for high_risk and low_risk respectively.

![CC](https://github.com/ssathyanath/Credit_Risk_Analysis/blob/main/Images/Undersampling.PNG)

- SMOTEENN
The balanced accuracy score was 0.64. Precision for high_risk was 0.01 and low_risk was 1.0. Sensitivity was 0.72 and 0.57 for high_risk and low_risk respectively.

![SMOTEENN](https://github.com/ssathyanath/Credit_Risk_Analysis/blob/main/Images/Combined.PNG)

- BalancedRandomForest Classifier
The balanced accuracy score was 0.79. Precision for high_risk was 0.03 and low_risk was 1.0. Sensitivity was 0.70 and 0.87 for high_risk and low_risk respectively.

![BCRF](https://github.com/ssathyanath/Credit_Risk_Analysis/blob/main/Images/BalancedRF.PNG)

- EasyEnsemble Classifier
The balanced accuracy score was 0.93. Precision for high_risk was 0.09 and low_risk was 1.0. Sensitivity was 0.92 and 0.94 for high_risk and low_risk respectively.

![EE](https://github.com/ssathyanath/Credit_Risk_Analysis/blob/main/Images/EEC.PNG)

## Summary

For credit card risk analysis resampling the data using RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN models and then using logistic regression to predict the results did not yield very good results. BalancedRandomForest Classifier and EasyEnsemble Classifier had much better results compared to the resampling models. Based on the above results, it is recommended to use the EasyEnsemble Clasiifier model. This model had the highest balanced accuracy, sensitivity and precision compared to other models.