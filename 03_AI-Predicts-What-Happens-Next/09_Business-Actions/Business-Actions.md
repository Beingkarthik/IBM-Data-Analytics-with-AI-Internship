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

## 500-Customer Decision Activity

Imagine that the business has 500 customers and must choose between two churn prediction models.

### Model A — Higher Recall

Model A identifies more customers who are actually at risk of churn.

Advantages:

- Fewer actual churned customers are missed.
- More customers can receive retention actions.
- Useful when missing a churned customer is expensive.

Disadvantage:

- It may identify more customers who do not actually churn.
- This can increase retention campaign costs.

### Model B — Higher Precision

Model B is more accurate when it predicts that a customer is at risk.

Advantages:

- Fewer unnecessary retention actions.
- Marketing resources can be focused on customers more likely to churn.
- Useful when retention campaigns are expensive.

Disadvantage:

- It may miss more customers who are actually at risk.

## Which Model Should the Business Choose?

There is no universal answer.

The choice depends on the business cost of:

- False positives — contacting customers who would not churn.
- False negatives — missing customers who actually churn.

If missing a churned customer is more expensive, the business may prefer the higher-recall model.

If retention campaigns are expensive and unnecessary outreach must be minimized, the business may prefer the higher-precision model.

## Decision for This Project

The final project model prioritizes recall because identifying more potentially churned customers was considered important for customer-retention actions.

The selected Balanced + Scaled Logistic Regression model achieved:

```text
Recall = 90.00%
Precision = 41.86%
