# Final Project - Supermarket Sales Analysis

## 1. Project Overview

This project analyzes 500 supermarket sales transactions to understand sales performance, customer behavior, product performance, payment preferences, branch performance, and monthly sales trends.

## 2. Dataset

- Total Transactions: 500
- Total Columns: 13
- Date Range: January 1, 2026 to July 1, 2026
- Missing Values: 0
- Duplicate Rows: 0

## 3. Data Validation

The dataset was checked for missing values and duplicate records.

Sales consistency was verified using:

Quantity × Unit Price = Sales

The maximum difference between the calculated sales and the existing Sales column was approximately 4.55 × 10^-13, which is effectively zero and is due to floating-point precision.

## 4. Overall Results

| Metric | Result |
|---|---:|
| Total Sales | ₹244,411.08 |
| Average Sales | ₹488.82 |
| Total Quantity Sold | 2,768 |
| Total Transactions | 500 |
| Average Rating | 3.99 / 5 |

## 5. Branch Analysis

Branch C (Mumbai) generated the highest total sales.

| Branch | Sales |
|---|---:|
| C | ₹72,469.45 |
| B | ₹64,116.26 |
| D | ₹55,468.29 |
| A | ₹52,357.08 |

## 6. Category Analysis

Beverages generated the highest sales.

| Category | Sales |
|---|---:|
| Beverages | ₹56,108.24 |
| Personal Care | ₹45,943.96 |
| Dairy | ₹43,992.00 |
| Grocery | ₹40,470.47 |
| Fruits | ₹23,263.17 |
| Snacks | ₹16,992.97 |
| Vegetables | ₹11,124.17 |
| Bakery | ₹6,516.10 |

Beverages also had the highest quantity sold with 465 units.

## 7. Product Analysis

Cheese was the highest-selling product with ₹27,906.30 in sales.

Potato had the highest quantity sold among individual products with 194 units.

## 8. Payment Method Analysis

UPI was the most-used payment method with 127 transactions.

UPI also generated the highest payment-method sales at ₹67,910.33.

| Payment Method | Transactions | Sales |
|---|---:|---:|
| UPI | 127 | ₹67,910.33 |
| Net Banking | 126 | ₹65,194.93 |
| Card | 125 | ₹57,265.64 |
| Cash | 122 | ₹54,040.18 |

## 9. Customer Analysis

Members generated higher total sales than Normal customers.

| Customer Type | Sales |
|---|---:|
| Member | ₹143,009.30 |
| Normal | ₹101,401.78 |

Average sales per transaction:

- Member: ₹483.14
- Normal: ₹497.07

## 10. Monthly Sales Analysis

April 2026 recorded the highest monthly sales.

| Month | Sales |
|---|---:|
| January | ₹43,415.53 |
| February | ₹30,068.15 |
| March | ₹37,306.42 |
| April | ₹52,569.77 |
| May | ₹42,542.31 |
| June | ₹35,041.46 |
| July | ₹3,467.44 |

Note: July contains transactions only through July 1, so it should not be interpreted as a complete-month decline.

## 11. Rating Analysis

The overall average customer rating was 3.99/5.

Bakery had the highest average category rating at approximately 4.24/5.

## 12. Visualizations

The project includes:

1. Sales by Branch
2. Sales by Category
3. Monthly Sales Trend
4. Sales by Payment Method
5. Sales by Customer Type
6. Quantity Sold by Category
7. Sales by Product

## 13. Key Business Insights

- Branch C is the strongest-performing branch by total sales.
- Beverages is the leading category by sales and quantity.
- Cheese is the highest-selling product by sales.
- Potato has the highest quantity sold among individual products.
- UPI is the most-used payment method and generates the highest payment-method sales.
- Members contribute higher total sales than Normal customers.
- April has the highest recorded monthly sales.
- Bakery has the highest average category rating.

## 14. Business Recommendations

- Maintain sufficient inventory for high-selling categories such as Beverages.
- Monitor Cheese and other high-performing products to avoid stock shortages.
- Study Branch C's performance and identify practices that can be applied to other branches.
- Continue supporting UPI and other digital payment options.
- Use membership programs and customer engagement strategies to maintain Member sales.
- Monitor monthly sales trends while considering incomplete periods such as July.

## 15. Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- OpenPyXL
- Jupyter Notebook

## 16. Conclusion

The supermarket sales analysis provides a clear view of sales performance across branches, categories, products, customers, payment methods, and time periods. The results can support inventory planning, customer engagement, payment strategy, and branch-level business decisions.
