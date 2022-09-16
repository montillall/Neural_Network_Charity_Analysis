# Neural_Network_Charity_Analysis

## Overview 

A CSV from Alphabet Soup, has been provided containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization.

Using machine learning and neural networks, it is required to use the features in the provided dataset to help create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.


## Results
The results of the study is described as follows:

### Data Prepocessing

* What variable(s) are considered the target(s) for your model?
The target variable considered for the model is: IS_SUCCESSFUL
* What variable(s) are considered to be the features for your model?
The feature variables for the model are: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT
* What variable(s) are neither targets nor features, and should be removed from the input data?  
The non-beneficial variables are: EIN, NAME

### SMOTE Oversampling

![](Resources/SMOTE_Oversampling.png)

* Balanced Accuracy Score: 65%
* Precision: for high risk loans, the precision is low at 1% and high for low risk loans at 100%
* Recall: for high risk loans, the recall is 64% and for low risk loans at 65%

### Undersampling

![](Resources/Undersampling.png)

* Balanced Accuracy Score: 65%
* Precision: for high risk loans, the precision is low at 1% and high for low risk loans at 100%
* Recall: for high risk loans, the recall is 61% and for low risk loans at 45%


### Combination (Over and Under) Sampling

![](Resources/Combination_(Over_and_Under)_sampling.png)

* Balanced Accuracy Score: 64%
* Precision: for high risk loans, the precision is low at 1% and high for low risk loans at 100%
* Recall: for high risk loans, the recall is 70% and for low risk loans at 57%


### Balanced Random Forest Classifier

![](Resources/BalancedRandomForestClass.png)

* Balanced Accuracy Score: 79%
* Precision: for high risk loans, the precision is low at 4% and high for low risk loans at 100%
* Recall: for high risk loans, the recall is 67% and for low risk loans at 91%


### Easy Ensemble AdaBoost Classifier

![](Resources/EasyEnsembleClass.png)

* Balanced Accuracy Score: 93%
* Precision: for high risk loans, the precision is low at 7% and high for low risk loans at 100%
* Recall: for high risk loans, the recall is 91% and for low risk loans at 94%

## Summary
Looking at the results of the six models, the EasyEnsembleClassifer model resulted with an accuracy of 93% and a precision of 7% for High Risk loans, the recall was also high with this model compared to the others with a rate of 91%. For the Low Risk loans, the recall was also high with a rate of 94%. Given the better results of this model compare to the others, it is recommended to use this model for making predictions of credit risk
