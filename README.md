# Credit_Risk_Analysis

## Purpose

The purpose for this analysis is to utilize THREE different techniques to train and evaluate models with Unbalanced classes by using imbalanced-learn and scikit-learn.  For this Challenge, OVERSAMPLING the credit data was done using RandomOverSample and SMOTE(SYNTHETIC MINORITY OVERSAMPLING TECHNIQUE), which is a statinstcal technique for increasing the number of cases in your dataset in a balanced way.  It generates new instances from existing minority cases that the original data suppies as input.

UnderSampling was also used on the data, i.e. ClusterCentroids and SMOTEENN.  I analyzed the data and compared the 2 algorithm to predict credit risk.

###Deliverable 1:  Use Resampling Models to Predict Credit RIsk

For Deliverable 1, I was slates to evaluate THREE machine learning models by using resampling to determine if any of the models (RandomOverSampling, SMOTE, and ClusterCentroids) are better for determing credit risk.

#### RandomOverSampling Results

  ![image](https://user-images.githubusercontent.com/8845050/183158792-09c4c4c9-8b2f-4aa4-89c4-4064697b0e4e.png)

#### SMOTE Results

  ![image](https://user-images.githubusercontent.com/8845050/183158888-11b025c4-d144-4fcd-91c8-b758bb158d57.png)
  
#### ClusterCentroid Results

  ![image](https://user-images.githubusercontent.com/8845050/183159150-e5c9e425-b72e-4828-9996-c669c252bcaf.png)


## Results

##### Accuracy = (True Positive + True Negative) / (All Positives + All Negatives)

  - Accurancy:  
    - RandomSampling score = 0.65
    - ClusterCentroid score = 0.53(Lowest)
    - SMOTE score = 0.64
  







