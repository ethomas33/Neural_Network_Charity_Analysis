# Neural networks and deep learning 

## Overview of the analysis: 
In this code we are attempting to help a foundation predict where to make investments in organizations that will carry on their missions into the future.


## Results: 
The initial data set had the following columns: 
- EIN and NAME — Identification columns
- APPLICATION_TYPE — Alphabet Soup application type
- AFFILIATION — Affiliated sector of industry
- CLASSIFICATION — Government organization classification
- USE_CASE — Use case for funding
- ORGANIZATION — Organization type
- STATUS — Active status
- INCOME_AMT — Income classification
- SPECIAL_CONSIDERATIONS — Special consideration for application
- ASK_AMT — Funding amount requested
- IS_SUCCESSFUL — Was the money used effectively


### Data Preprocessing

#### Target model: 
- IS_SUCESSFUL

#### Features of the model:
- APPLICATION_TYPE
- AFFILIATION
- CLASSIFICATION
- USE_CASE
- ORGANIZATION
- STATUS
- INCOME_AMT
- SPECIAL_CONSIDERATIONS
- ASK_AMT

#### To be removed:
- EIN and NAME


### Compiling, Training, and Evaluating the Model
For this analysis I used 2 hidden layers that used the relu activation function, this is to help speed up the process. The two hidden layers contained 80 and then 30 neurons. Then one output layer that used the sigmoid activation function because this is a binary classification.

![DefineModel](https://github.com/ethomas33/Neural_Network_Charity_Analysis/blob/038d95aa41b91bc9f59ffecca5a1cab450330500/Challenge/Resources/DefineModel.PNG)

Attempts were made using different activation functions, increased number of neurons and the addition and subtraction of hidden layers but nothing seemed to help improve the models performance. 

## Summary: 
In summary the model was unable to reach the desired 75% accuracy. Expanding the type of machine learning could potentially help increase this accuracy. The next thing I would try is a decision tree model which generated a series of classified outputs.  