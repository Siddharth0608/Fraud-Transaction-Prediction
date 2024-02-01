# Fraud Transaction Prediction Model using Random Forest Classification

## Overview
This repository contains a machine learning model to predict fraudulent transactions for a financial company. The model is based on a binary classification problem, implemented using the Random Forest Classification algorithm from the scikit-learn library.

## Code Structure

### Data Preprocessing:

Reading the dataset from a CSV file.
Handling insignificant attributes like 'step,' 'type,' 'nameOrig,' and 'nameDest.'
Checking for missing values (null) in the dataset.

### Handling Imbalanced Data:

Addressing the highly unbalanced dataset by sampling a subset of non-fraudulent transactions.
Balancing the dataset to have a reasonable number of both fraud and non-fraud instances.
### Feature Engineering:

Adding two new attributes, 'balDiffOri' and 'balDiffDest,' representing the balance difference of the sender and receiver before and after the transaction.

### Data Splitting:

Splitting the dataset into training and testing sets.

### Model Training:

Initializing and training the Random Forest Classification model.
Evaluating the initial performance using accuracy, precision, and recall.

### Hyperparameter Tuning:

Performing hyperparameter tuning using RandomizedSearchCV to find the best combination of parameters for the Random Forest model.

### Model Evaluation:

Estimating the performance of the best model obtained from hyperparameter tuning.
Using confusion matrix and metrics like accuracy, precision, and recall.

### Feature Importance Analysis:

Plotting a bar graph to visualize the importance of features in predicting fraudulent transactions.
Prevention Strategies

### The model suggests the following prevention strategies based on feature importance:

Limiting the amount customers can withdraw or debit in a single transaction.
Implementing restrictions on large transactions for users who don't typically make significant transactions.

### Future Steps

Continuous monitoring of fraudulent transactions after implementing prevention measures.
Analyzing the effectiveness of prevention strategies over time.
Feel free to use and contribute to this repository to enhance fraud detection and prevention in financial transactions.
