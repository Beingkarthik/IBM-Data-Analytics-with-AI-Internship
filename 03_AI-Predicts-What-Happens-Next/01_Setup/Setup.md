# Setup — AI Predicts What Happens Next

## Masterclass

Masterclass 3 — AI Predicts What Happens Next

## Objective

The objective of this masterclass is to use customer transaction data to build a customer churn prediction workflow.

The workflow includes:

- Customer-level data creation
- RFM feature creation
- Churn definition
- Target leakage checking
- Logistic regression
- Model evaluation
- Churn probability
- Customer risk levels
- Business actions

## Dataset

The cleaned e-commerce dataset created during Masterclass 1 will be used.

The original dataset will not be modified.

## Tools

- Google Colab
- Python
- Pandas
- Scikit-learn
- Gemini

## Main Dataset Columns

- Order_ID
- Order_Date
- Customer_ID
- Product
- Category
- Region
- Quantity
- Revenue
- Profit

## Project Workflow

Cleaned Dataset
↓
Customer-Level Dataset
↓
RFM Features
↓
Churn Target
↓
Leakage Check
↓
Prediction Model
↓
Model Evaluation
↓
Churn Probability
↓
Customer Risk Level
↓
Business Actions

## Important Note

Target leakage must be checked before building the prediction model.

Prediction features must not contain information that directly reveals the target.

