# Credit_Risk_Analysis

## Project Overview & Purpose:

### Project Overview:

All around the world people borrow money to purchase homes or cars start businesses & peruse education. Loans are an essential part of modern society. But loans represent an opportunity & challenge to banks and other lending institutions. On one hand loans create revenue with the interest they generate on the other hand there is a risk that borrowers won’t repay their loans and banks loose their money. Banks have traditionally relied on measures like income, credit scores and collateral assets to asses lending risk but the rise of financial technology fintech has enabled users to use machine learning to analyze risk. Machine learning can look up a huge amount of data to arrive at a single decision. 
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

### Purpose of Analysis:

Fastlending is a peer-to-peer lending services company wants to use machine learning to predict credit risk. It is believed that using machine learning will provide a more accurate identification of good candidates for loans, which will lead to decrease in defaulted loans.

### Analysis Process: 

I will be using the credit card credit dataset from LendingClub for this analysis. I will need to dot he following:
1-	Oversample the data using the RandomOverSampler and SMOTE algorithms, 
2-	Undersample the data using the ClusterCentroids algorithm.
3-	Then, use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. 
4-	Next, I’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 
5-	Once done, I’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results:

### Oversample:
#### Naive Random OverSampler
Balanced Accuracy score: 0.64


#### SMOTE
Balanced Accuracy score: 0.63

### Undersample:
#### ClusterCentroids
Balanced Accuracy score: 0.51
### Combination of Oversample and undersample approach:
#### SMOTEENN
Balanced Accuracy score: 0.65

## Summary:
Balanced accuracy uses sensitivity and specificity to evaluate the performance of a classifier. The balanced accuracy is placed on a scale of 0 to 1. The closer to 1 the balanced accurracy is, the better the prediction of the model. For the credit card risk data set, all of the classifiers tested showed similar recall scores, and all had precision scores as low for high-risk loans and high for low-risk loans. The difference in these machine learning models occurs in the balanced accuracy score. The Easy Ensemble Classifier outperformed all off the other models significantly with a score of 0.93. Seeing as none of the other machine learning models had balanced accuracy scores above 0.78, the Easy Ensemble Classifier is the best choice when analyzing and predicting credit card risk.
