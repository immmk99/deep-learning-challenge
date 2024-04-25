# Module 21: Deep Learning Challenge

## Overview
This report documents the construction of a TensorFlow Keras neural network model, leveraging data sourced from Alphabet Soup, a nonprofit organization. The primary aim of this model is to identify applicants with the highest likelihood of success upon receiving funding.
From Alphabet Soup’s business team, we have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:
- EIN and NAME—Identification columns
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organization classification
- USE_CASE—Use case for funding
- ORGANIZATION—Organization type
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special considerations for application
- ASK_AMT—Funding amount requested
- IS_SUCCESSFUL—Was the money used effectively

## Results
**Data Processing**
Target Variables:
- IS_SUCCESSFUL

Features Variables:
- APPLICATION_TYPE
- AFFILIATION
- CLASSIFICATION
- USE_CASE
- ORGANIZATION
- STATUS
- INCOME_AMT
- ASK_AMT

Removed from input data:
- EIN and NAME
- SPECIAL_CONSIDERATIONS

**Compiling, Training, and Evaluating the Model**
How many neurons, layers, and activation functions did you select for your neural network model, and why?
The first model contains 2 layer, an additional layer was added to optimize the perfomance.
Were you able to achieve the target model performance?
The first model is close to hitting the target performance with an accuracy of 0.729912519454956
After using various optimization method, the highest accuracy I was able to achieve is of 0.7268804907798767 which is lower than the simpler model.
What steps did you take in your attempts to increase model performance?
- binned unnecessary variables
- added a layer to the neural network
- increased the number of neurons

## Summary
The model seems to have achieved moderate performance with an accuracy of approximately 72.7%, indicating that it can correctly classify applicants with a certain level of success. However, further analysis, such as examining precision, recall, and F1-score, along with potential improvements to the model architecture or data preprocessing, may be necessary to enhance its effectiveness.
