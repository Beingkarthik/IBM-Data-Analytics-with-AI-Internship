# Business Actions — AI Predicts What Happens Next

## Objective

The business-action stage converts customer churn predictions and risk levels into practical retention actions.

The goal is to help the business prioritize customers based on their predicted churn risk.

## Customer Risk and Recommended Actions

| Risk Level | Customers | Recommended Action |
|---|---:|---|
| Low Risk | 108 | Continue regular customer engagement |
| Medium Risk | 234 | Use personalized offers and proactive engagement |
| High Risk | 22 | Prioritize immediate retention outreach and personalized offers |

## High-Risk Customer Action

The High Risk group contains 22 customers.

These customers have higher predicted churn probabilities and can be prioritized for retention activities.

Recommended actions include:

- Immediate retention outreach
- Personalized offers
- Direct customer engagement
- Monitoring future purchasing behavior
- Reviewing customer-specific activity before taking action

## Medium-Risk Customer Action

Medium Risk is the largest group with 234 customers.

Recommended actions include:

- Proactive customer engagement
- Personalized promotions
- Monitoring changes in purchase behavior
- Encouraging repeat purchases
- Reviewing customers whose risk level increases over time

## Low-Risk Customer Action

There are 108 Low Risk customers.

Recommended actions include:

- Continue normal engagement
- Maintain good customer service
- Encourage repeat purchases
- Monitor future customer behavior

## Model-Based Customer Prioritization

The model generated churn probabilities that can be used to prioritize customer retention efforts.

Examples of customers with high predicted churn probability include:

| Customer ID | Churn Probability | Risk Level |
|---|---:|---|
| C456 | 0.723789 | High Risk |
| C106 | 0.723203 | High Risk |
| C264 | 0.720680 | High Risk |
| C263 | 0.720528 | High Risk |
| C091 | 0.719764 | High Risk |
| C231 | 0.718654 | High Risk |
| C323 | 0.718564 | High Risk |
| C154 | 0.717714 | High Risk |
| C008 | 0.717010 | High Risk |
| C001 | 0.715966 | High Risk |

## Business Decision Framework

The recommended decision flow is:

```text
Customer Data
      ↓
Churn Prediction Model
      ↓
Churn Probability
      ↓
Risk Level
      ↓
Business Action
      ↓
Customer Retention


