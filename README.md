# Neural_Network_Charity_Analysis-

## Overview
In this project we use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

For this purpose we are creating a deep learning neural network model and optimize the model to achieve our target model performance.

## Deliverable 1 - Data Preprocessing
- The EIN and NAME columns have been dropped
- The columns with more than 10 unique values have been grouped together
- The categorical variables have been encoded using one-hot encoding
- The preprocessed data is split into features and target arrays
-  The preprocessed data is split into training and testing datasets
- The numerical values were standardized using the StandardScaler() module
- What variable(s) are considered the target(s) for your model? IS_SUCCESSFUL
- What variable(s) are considered to be the features for your model? 
APPLICATION_TYPE            17
AFFILIATION                  6
CLASSIFICATION              71
USE_CASE                     5
ORGANIZATION                 4
STATUS                       2
INCOME_AMT                   9
SPECIAL_CONSIDERATIONS       2
ASK_AMT                   8747
- What variable(s) are neither targets nor features, and should be removed from the input data? NAME and EIN

## Deliverable 2 - Compile, Train, and Evaluate the Model
### The neural network model using Tensorflow Keras contains working code that performs the following steps:
- The number of layers, the number of neurons per layer, and activation function are defined
- An output layer with an activation function is created
- There is an output for the structure of the model 
- There is an output of the model’s loss and accuracy
- The model's weights are saved every 5 epochs
The results are saved to an HDF5 file
- How many neurons, layers, and activation functions did you select for your neural network model, and why? 2 Hidden Layers with 30/25 neurons and relu activation function
- Were you able to achieve the target model performance? Couldn't achieve target model performance > 75%
- What steps did you take to try and increase model performance? 

Took the following steps to optimize the model in order to achieve a target predictive accuracy higher than 75%.

### Attempt 1
- Removed noisy features like "USE_CASE_Other","AFFILIATION_Other"
- Increased neurons in the hidden layers

### Attempt 2
- Increased number of hidden layers

### Attempt 3
- Changed the activation function for all the hidden layers to 'tanh'

## Summary
After making three attempts to optimize the neural network model, we couldn't achieve the target performance of > 75%. We could do a few or all of the following to achieve our target:

- Increase the number of epochs.
- Keep activation function as relu
- Remove noisy features like ORGANIZATION and USE_CASE
- Create Binning for AFFILIATION and INCOME_AMT






