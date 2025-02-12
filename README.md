# Customer-Churn-Prediction-Using-Keras

## Overview

This repository focuses on building a binary classification model to predict customer churn for a telecom company. By analyzing customer data, the project aims to identify patterns and factors that contribute to churn, enabling the company to take proactive measures to retain customers.

## Problem Statement

Customer churn is a critical issue in the telecom industry, where customers often switch to competitors. This project uses machine learning to predict whether a customer will churn based on features like tenure, monthly charges, and payment methods. The goal is to build accurate predictive models using Keras and TensorFlow.

## Dataset

The dataset contains customer information, including:
- **Demographics:** Gender, Senior Citizen status, Partner, Dependents
- **Services:** Internet Service, Online Security, Device Protection
- **Billing Information:** Monthly Charges, Total Charges, Payment Method
- **Target Variable:** Churn (1 = Yes, 0 = No)

For detailed column descriptions, refer to the [data dictionary](customer-churn-data-dictionary.xlsx).

## Key Features

1. **Data Manipulation:**
   - Analyze gender distribution and service usage.
   - Extract specific subsets of customers based on tenure or payment methods.

2. **Data Visualization:**
   - Pie charts for churn distribution.
   - Bar plots for Internet Service usage.

3. **Model Building:**
   - Sequential models using Keras with features like `tenure`, `MonthlyCharges`, and `TotalCharges`.
   - Dropout layers for regularization.
   - Performance evaluation using confusion matrices and accuracy vs. epochs graphs.

## Implementation Highlights

- **Model 1:** Predicts churn using `tenure` as the feature.
  - Input layer with 12 nodes (ReLU activation).
  - Hidden layer with 8 nodes (ReLU activation).
  - Optimized with Adam optimizer over 150 epochs.

- **Model 2:** Adds dropout layers for improved generalization.
  - Dropout after input (0.3) and hidden layers (0.2).

- **Model 3:** Uses multiple features (`tenure`, `MonthlyCharges`, `TotalCharges`) for better predictions.

- ## Results

The models demonstrate how deep learning can effectively predict customer churn by leveraging structured data. The inclusion of dropout layers improves generalization, while multiple features enhance prediction accuracy.

This project provides a practical framework for addressing customer churn in industries where retention is critical.
