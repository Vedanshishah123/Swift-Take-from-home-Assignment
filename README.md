# Swift-Take-from-home-Assignment
# Customer Fraud Detection Model

This repository contains code and documentation for building and evaluating a fraud status of customers detection . The model uses various machine learning algorithms to predict fraudulent transactions based on customer data.

## Table of Contents

- [Overview](#overview)
- [Data](#data)
- [Models](#models)
  - [Random Forest](#random-forest)
  - [AdaBoost](#adaboost)
  - [Support Vector Machine (SVM)](#support-vector-machine-svm)
- [Hyperparameter Tuning](#hyperparameter-tuning)
- [Evaluation](#evaluation)


## Overview

This project involves the development of a  fraud status of customers detection model using several machine learning algorithms. The goal is to accurately classify cuatomers as fraudulent or non-fraudulent based on features extracted from customer data.

## Data

The dataset consists of two main CSV files:

### `customer_transaction_details.csv`
Contains transaction-level details

### `customers_df.csv`
Contains customer-level details.

## Models

### Random Forest

- **Description**: An ensemble learning method that constructs multiple decision trees and merges them to improve accuracy and control overfitting.
- **Key Results**:
  - **Classification Report**: Provides metrics such as precision, recall, and F1-score for both classes.
  - **Training Accuracy**: 0.99
  - **Testing Accuracy**: 0.81

### AdaBoost

- **Description**: A boosting technique that combines the outputs of several weak classifiers to create a strong classifier. It focuses on misclassified instances to improve model performance.
- **Key Results**:
  - **Classification Report**: Includes precision, recall, and F1-score for each class.
  - **Overall Accuracy**: 0.81

### Support Vector Machine (SVM)

- **Description**: A classification method that finds the optimal hyperplane to separate classes. It is effective for high-dimensional spaces and can handle non-linearly separable data.
- **Key Results**:
  - **Classification Report**: Details precision, recall, and F1-score for each class.
  - **Training Accuracy**: 0.82
  - **Testing Accuracy**: 0.86

## Hyperparameter Tuning

Hyperparameter tuning was performed using Grid Search to optimize model performance. For SVM, the best parameters were found to be `C = 10` and `kernel = 'rbf'`, resulting in a mean cross-validation score of 0.797.

## Evaluation

The models were evaluated using various metrics including accuracy, precision, recall, and F1-score. The SVM model showed strong performance with an accuracy of 86% on the test set, indicating its effectiveness in
