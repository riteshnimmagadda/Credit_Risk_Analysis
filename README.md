# Credit_Risk_Analysis

## Overview of the analysis
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, this analysis is to employ different techniques to train and evaluate models with unbalanced classes. Imbalanced-learn and scikit-learn libraries are used to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, this project oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, it compares two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Towards the end,we will evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results
* Naive Random Oversampling

  * Balanced Accuracy Score is 65.7%
  * Precision Score is 1%
  * Recall Score is 71%

![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/balanced%20accuracy%20score.png)
![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/imbalanced%20classification%20report.png)
![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/confusion%20matrix.png)

* SMOTE Oversampling
  *  Balanced Accuracy Score is 66.22%
  *  Precision Score is 1%
  *  Recall Score is 63%
 
![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/SMOTE_balanced%20accuracy%20score.png)

![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/SMOTE_confusion%20matrix.png)

![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/SMOTE_imbalanced%20classification%20report.png)

* Undersampling
  * Balanced Accuracy Score is 54.42%
  * Precision Score is 1%
  * Recall Score is 69%

![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/under_balanced%20accuracy%20score.png)

![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/under_confusion%20matrix.png)

![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/under_imbalanced%20classification%20report.png)

* Combination
  * Balanced Accuracy Score is 64.47%
  * Precision Score is 1%
  * Recall Score is 72%

![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/combi_balanced%20accuracy%20score.png)

![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/combi_confusion%20matrix.png)

![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/combi_imbalanced%20classification%20report.png)


* Balanced Random Forest Classifier
  * Balanced Accuracy Score is 78.85%
  * Precision Score is 3%
  * Recall Score is 70%

![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/elbalanced%20accuracy%20score.png)

![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/el_confusion%20matrix.png)

![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/el_imbalanced%20classification%20report.png)

* Easy Ensemble AdaBoost Classifier
  * Balanced Accuracy Score is 93.16%
  * Precision Score is 3%
  * Recall Score is 70%

![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/ee_balanced%20accuracy%20score.png)

![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/ee_confusion%20matrix.png)

![alt_text](https://github.com/riteshnimmagadda/Credit_Risk_Analysis/blob/main/Resources/ee_imbalanced%20classification%20report.png)

## Summary
From the above analysis Balanced Random Forest Classifier and Easy Ensemble AdaBoost Classifier has the highest Balanced Accuracy Scores with 78.85% and 93.16% and the recommended for the predection analysis.
