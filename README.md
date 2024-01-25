# Credit Risk Classification

## Overview of the Analysis
The purpose of this analysis was to train a logical regression model to determine an individuals credit worthiness based on their financial information. 

Using an individual's; 'loan_size', 'interest_rate', 'borrower_income', 'debt_to_income','num_of_accounts', 'derogatory_marks', 'total_debt', we trained a logical regression model by comparing those factors to the 'loan_status' of the individual. This should create a model that is able to predict whether or not a indivdual should take out a loan based on the given information. 

## Process 
A csv file is loaded as dataframe which is then split into X and Y, where Y is the loan status and X is all the other factors. Then further split into a 'train' and 'test' set using sklearn module, a logical regression model is then fitted to the train dataset and then using the X test data for prediction.

## Results
##### Logical Regression Model:
    * Overall accuracy: 0.9924164259182832
    ---------------------------------------
    * Precision Class 0: 0.9960462646052166
    * Recall Class 0: 0.9952827407276372
    ---------------------------------------
    * Precision Class 1: 0.8746081504702194
    * Recall Class 1: 0.8928

## Summary
The model is fairly accuracte at 99% overall accuracy. The model seem to almost perfectly predict class '0' at 99% precision and recall but in this situation it would be best if the model perfomed better with classifying class '1'. As class '1' is determine to be 'high-risk' loans, but it precision and recall are both good at 87% and 89% respectively. 

The model is defintely usable but improvement on precision and accuracy for class '1' can be made as individuals at high-risk shouldn't be allowed to make loans as it could negatively impact both the individual and the loan company. 