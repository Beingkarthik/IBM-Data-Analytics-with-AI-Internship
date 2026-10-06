# Risk Analysis — AI Predicts What Happens Next

## Objective

The risk analysis stage converts predicted customer churn probabilities into practical customer risk levels.

The purpose is to identify customers who may require attention and support business retention decisions.

## Risk Level Distribution

The model-generated customer risk levels were distributed as follows:

| Risk Level | Customers | Percentage |
|---|---:|---:|
| Low Risk | 108 | 29.67% |
| Medium Risk | 234 | 64.29% |
| High Risk | 22 | 6.04% |

The majority of customers fall into the Medium Risk category, while 22 customers are classified as High Risk.

## High-Risk Customer Identification

Customers with higher predicted churn probability were identified as high-risk customers.

The highest predicted churn probabilities included:

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

## Customer Risk Interpretation

### Low Risk

Customers in the Low Risk category have relatively lower predicted churn probability.

These customers can continue through normal customer engagement and service processes.

### Medium Risk

Medium Risk contains the largest customer group with 234 customers.

These customers may benefit from regular engagement, personalized offers, and continued monitoring of their purchasing behavior.

### High Risk

There are 22 High Risk customers.

These customers have higher predicted churn probabilities and should receive priority attention through retention-focused actions.

## Recommended Business Actions

| Risk Level | Recommended Action |
|---|---|
| Low Risk | Continue regular engagement |
| Medium Risk | Personalized offers and increased engagement |
| High Risk | Immediate retention outreach and personalized offers |

## Important Interpretation Note

The risk levels are based on model-predicted churn probabilities.

A High Risk classification does not mean that a customer will definitely churn. It indicates that the model estimates a higher probability of churn based on the selected customer features.

Therefore, the predictions should support business decision-making rather than replace human judgment.

## Model Evaluation Context

The initial scaled model achieved:

- Accuracy: 0.7260
- Precision: 0.0000
- Recall: 0.0000

The balanced model achieved:

- Accuracy: 0.6301
- Precision: 0.4186
- Recall: 0.9000

The balanced model was able to identify a much larger proportion of the churn class, with a recall of 0.90.

However, its precision was 0.4186, meaning that some customers classified as churn-risk may not actually churn.

## Conclusion

The risk analysis transforms model predictions into actionable customer risk categories.

The analysis identified:

- 108 Low Risk customers
- 234 Medium Risk customers
- 22 High Risk customers

The High Risk group can be prioritized for retention activities, while Medium Risk customers can receive proactive engagement.

The model predictions should be validated with additional customer behavior and business data before making final retention decisions.

