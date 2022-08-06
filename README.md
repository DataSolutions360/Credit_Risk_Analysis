# Credit_Risk_Analysis

## Purpose

The purpose for this analysis is to utilize THREE different techniques to train and evaluate models with Unbalanced classes by using imbalanced-learn and scikit-learn.  For this Challenge, OVERSAMPLING the credit data was done using RandomOverSample and SMOTE(SYNTHETIC MINORITY OVERSAMPLING TECHNIQUE), which is a statinstcal technique for increasing the number of cases in your dataset in a balanced way.  It generates new instances from existing minority cases that the original data suppies as input.

UnderSampling was also used on the data, i.e. ClusterCentroids and SMOTEENN.  I analyzed the data and compared the 2 algorithm to predict credit risk.

### Deliverable 1:  Use Resampling Models to Predict Credit Risk

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


  - Precision:
  
    - RandomOverSampling: High Risk precision is low; Low Risk precision is high
    - SMOTE: High Risk precision is low; Low Risk precision is high
    - ClusterCentroid: High Risk precision is low; Low Risk precision is high

  - Recall Score:
  
    - The recall score between all three models are as follows:
    
          - RandomOverSampling:  High Risk is 0.62; Low Risk is 0.68
          - SMOTE: High Risk precision is low; Low Risk precision is high
          - ClusterCentroid: High Risk precision is the lowest of the 3 being 0.59 and 0.44 respectively.
    
    - The RandomOverSampling model had a mich higher score than SMOTE and the lowest recall score was from the ClusterCentroid with a recall score of 0.44

### Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk

For Deliverable 2, I used the combined approach of over and under-sampling with the SMOTEENN algorithm to determine if these results form a better approach at predicting the results from Deliverable 1.

#### SMOTEENN Results

![image](https://user-images.githubusercontent.com/8845050/183235313-f8741970-af3b-4733-9bbc-f65279b20468.png)

## Results

  - Accuracy:  The accuracy of SMOTEENN model is 0.68 = [48 + 11709] / [48 39 + 5409 + 11709]
  
  - Precision: The precision for high risk is low and the low risk precision is high
  
  - Recall score:
      - The high risk score is 0.59
      - The low risk score is 0.66

### Deliverable 3: Use Ensemble Classifier to Predict Credit Risk

For Deliverable 3, I used the "IBLEARN.ENSAMBLE" library to train and compare two different classifiers (BalancedRandomForestCLassifier, and EasyEnsambleClassifier) to predict credit risk.

#### BalancedRandomForestClassifier Results

![image](https://user-images.githubusercontent.com/8845050/183253403-c3fa0edb-968c-4715-b74c-27043a1d4d30.png)

#### EasyEnsembleClassifer(AdaBoost) Results

![image](https://user-images.githubusercontent.com/8845050/183253469-891da54e-8a4f-41cc-a5b1-0af0454ff3ab.png)


## Results

  - Accurancy:
  
      - EasyEnsemble model scored the highest with 0.93
      - BalancedRandomForestClassifier had a score of 0.79

  - Precision:

      - The High Risk precision for BalancedRandomForestClassifier is *low* and the low risk is *high*
      - The High Risk precision for EasyEnsemble is low and the *low* risk is *high*.

  - Recall Scores:

      - The high risk score for BalancedRandomForestClassifier is *low* and the low risk is *high*
      - The high risk score for EasyEnsemble is *high* and the low risk is *high*


## Summary

  Of the 6 models being used, it is my opinion that EasyEnsembleClassifier model is the best fit for the data and possibly more robust(sensitivity score allowing for different data sets), while accuracy of 0.90+ is a primary indicator for this, the others averaged around 0.80, which is substantially lower.
  
  The precision between all the models was similar, so that was NOT a deciding factor, in my opinion.  The recall score for the EasyEnsembleClassifier was the best, with both a LOW RISK and HIGH RISK offering in the 0.90's.  The RandomOverSampling, SMOTE, CLusterCentroid models do NOT come close to being as precise, as the ranges were 0.50 to 0.65 overall.  
  
  I would choose EasyEnsembleClassifier going forward, for this data set.
  
  
  ## Resources
    - Jupyter Notebook
    - Pandas
    - Numpy
    mnlev(virtual environment)
  
  
  










       







