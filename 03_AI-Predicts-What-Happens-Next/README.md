# AI Predicts What Happens Next

## Overview

This project uses customer transaction data and machine learning to predict customer churn risk.

The analysis transforms historical customer behavior into:

- Customer-level data
- RFM features
- Churn prediction
- Model evaluation
- Churn probability
- Customer risk levels
- Business retention actions

## Objective

The objective is to identify customers who may be at risk of churn and prioritize them for appropriate retention activities.

## Dataset

The project uses the cleaned e-commerce dataset prepared during Masterclass 1.

Customer-level features were created from transaction history.

The final model dataset contains:

- 364 historical customers
- 4 prediction features
- 1 churn target

## Key Features

The prediction model uses:

- Recency
- Frequency
- Monetary
- Avg_Order_Value

## Machine Learning Model

A Logistic Regression classification model was used to predict customer churn.

The target variable is:

```text
Churn_Status


