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

### Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why?
For the initial model, 2 hidden layers were included with 80 and 30 neurons, respectively. Both layers used relu as activation since it does better with nonlinear data and for the output layer, 1 neuron with activation sigmoid

* Were you able to achieve the target model performance?
The results of the initial model showed and accuracy of 74.11% and when evaluated with the test data the accuracy resulted in 72.53% 

* What steps did you take to try and increase model performance?
In order to optimize the model, several steps and attemps were tested including:
  Dropping SPECIAL_CONSIDERATIONS feature
  Added one additional hidden layer
  Increased number of neurons for each hidden layer to 100, 80, 80
 Results showed no improvement in the performance of the model


## Summary
In summary, the deep neural network classification model generated to predict loan applicant success provided in the charity_data.csv showes a 72.53% accuracy, which does not reach the 75% accuracy target. The optimization methods applied the the initial model do not show any significant improvements in the model
