# Credit_Risk_Analysis

## Background <br>
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. In this module challenge, I used different techniques to train and evaluate models with unbalanced classes. <br>

## Overview of the analysis: Explain the purpose of this analysis <br>
In this project analysis, I use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. I use three different approaches with the dataset from LendingClub where, in a nutshell, I oversample the data using the RandomSampler and SMOTE algorithm, undersample the data using the ClusterCentroid algorithm and use a combination of both undersampling and oversampling using the SMOTEEN algorithm. <br>

## Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results

### Naive Random Oversampling
Balanced Accuracy: 0.7844011748069183
Precision: The precision is low for high_risk loans and is high for low_risk loans.
Recall: High risk: .60 and low risk: .65

![Naive Random Oversampling](https://github.com/jinnabelle/Credit_Risk_Analysis/blob/main/Random%20Oversampling.png)

### SMOTE Oversampling
Balanced Accuracy: 0.6512584051472337
Precision: The precision is low for high_risk loans and is high for low_risk loans.
Recall: High risk: .64 and Low risk: .66

![Smote Oversampling](https://github.com/jinnabelle/Credit_Risk_Analysis/blob/main/SMOTE%20Oversampling.png)

### Undersampling
Balanced Accuracy: 0.5902911232781787
Precision: The precision is low for high_risk loans and is high for low_risk loans.
Recall: High risk:.59 and low risk:.43

![Undersampling](https://github.com/jinnabelle/Credit_Risk_Analysis/blob/main/Undersampling.png)

### Combination (Over and Under) Sampling
Balanced Accuracy: 0.5103017191018931
Precision: The precision is low for high_risk loans and is high for low_risk loans.
Recall: High risk: .70 and low risk:.57

![Combination Over and Under Sampling](https://github.com/jinnabelle/Credit_Risk_Analysis/blob/main/Combination%20(Over%20and%20Under)%20sampling.png)

### Balanced Random Forest Classifier
Balanced Accuracy: 0.7844011748069183
Precision: The precision is low for high_risk loans and is high for low_risk loans.
Recall: High risk: .68 and low risk:.89

![Balanced Random Forest Classifier](https://github.com/jinnabelle/Credit_Risk_Analysis/blob/main/Balanced%20Random%20Forest%20Classifier.png)

### AdaBoost Classifier
Balanced Accuracy: 0.925427358175101
Precision: The precision is low for high_risk loans and is high for low_risk loans.
Recall: High risk: .91 and low risk: .94

![Adaboost Classifier](https://github.com/jinnabelle/Credit_Risk_Analysis/blob/main/AdaBoost%20Classifer.png)

## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

Combination Sampling had the worst accuracy compared to the other five machinese learning models with .51 accuracy. Undersampling had a slightly better accuracy with 0.59, then SMOTE oversampling with 0.65. Naive Random Sampling and the balanced Random Forest classifier had similar accuracy with 0.78. And the easy ensemble AdaBoost classifier had the highest accurance of 0.92. As far as precision goes, all the models performed very similarly where the precision is low for high risk loans and high for low risk loans. Because of these two factors, I would recommend using the Easy Ensemble AdaBoost classifer as it had the highest accuracy compared to the rest of models used in this project.
