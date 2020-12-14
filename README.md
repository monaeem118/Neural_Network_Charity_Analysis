# Neural_Network_Charity_Analysis

## Overview

The purpose of this assignment is to perform loan prediction risk analysis using the knowledge of machine learning and neural networks.

## Results

### Data Preprocessing

- "IS_SUCCESSFUL" is considered as target variables for this model.
- Following variables are considered to be the feature variables for this model:
'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS'.
- 'EIN' and 'NAME' are neither targets nor features and should be removed from the input data.

### Compiling, Training and Evaluating the Model

- Layers Used = 1 <br>
- Neurons Used in Layer 1 = 99

- Rule of thumb is to have two to three times the amount of neurons in the hidden layer as the number of inputs. Number of inputs in first optimization "AlphabetSoupCharity_Optimization1.ipynb" is 33 so,

 - number_hidden_nodes = number_input_features * 3

- Was able to achieve accuracy of 67% in one optimization after removing "CLASSIFICATION" feature.

- Removed "CLASSIFICATION" from feature list and decreased number of layers.

- Used "relu" activation function in first layer for non-linear input and "sigmoid" function in output layer to achieve binary classification.

## Summary

Following are the accuracies achieved in each optimization:

Original code:
268/268 - 0s - loss: 6.8093 - accuracy: 0.4716
Loss: 6.809304237365723, Accuracy: 0.47160351276397705

First Optimization:
268/268 - 0s - loss: 0.7079 - accuracy: 0.6722
Loss: 0.7078773975372314, Accuracy: 0.6721866130828857

Second Optimization:
22/22 - 0s - loss: 2.2513 - accuracy: 0.5893
Loss: 2.2512712478637695, Accuracy: 0.589337170124054

Third Optimization:
268/268 - 0s - loss: 0.7853 - accuracy: 0.5433
Loss: 0.7852626442909241, Accuracy: 0.5433337092399597

Further data cleaning is required and one recommendation is to remove applications that have in-active status. 





