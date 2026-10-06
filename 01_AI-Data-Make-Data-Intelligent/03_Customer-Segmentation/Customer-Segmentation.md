# Customer Segmentation

## 1. Objective

The objective of customer segmentation is to group customers based on their transaction behaviour.

For this Masterclass 1 dataset, customers are classified into:

- New Customer
- Repeat Customer
- Unknown Customer

## 2. Segmentation Logic

The segmentation is based on the number of transactions associated with each `Customer_ID`.

| Condition | Customer Segment |
|---|---|
| Customer appears once | New Customer |
| Customer appears more than once | Repeat Customer |
| Customer_ID is missing | Unknown Customer |

## 3. Why Customer Segmentation Is Useful

Customer segmentation helps answer business questions such as:

- Who are the highest-value customers?
- Which customers are repeat customers?
- How many customers are new versus repeat?
- Which customer groups generate more revenue?
- Which customers may require additional attention?

These types of customer questions are part of the Masterclass 1 business-question framework. :chatgpt-content-reference{index="1"}

## 4. Customer Segment in the Dataset

A new column named `Customer_Segment` was added to the cleaned dataset.

Possible values are:

- `New Customer`
- `Repeat Customer`
- `Unknown Customer`

## 5. Important Consideration

Customers with missing `Customer_ID` values are not classified as new customers because there is not enough information to determine their transaction history.

They are classified as `Unknown Customer`.

## 6. Result

The `Customer_Segment` field is now available in `Cleaned_Dataset.xlsx` and can be used for further customer-level analysis.
