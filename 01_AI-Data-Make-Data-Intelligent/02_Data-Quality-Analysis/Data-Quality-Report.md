# Data Quality Analysis

## 1. Objective

The objective of this analysis is to identify data-quality problems in the raw e-commerce dataset before performing further analysis.

The Masterclass 1 framework identifies six major data-quality areas:

1. Missing Values
2. Duplicate Records
3. Inconsistent Categories
4. Incorrect Dates
5. Formatting Problems
6. Outliers

## 2. Dataset Size

The Raw_Data sheet contains:

- Rows: 2,000
- Columns: 9

## 3. Missing Values

The following missing values were identified:

| Column | Missing Values | Percentage |
|---|---:|---:|
| Order_ID | 0 | 0% |
| Order_Date | 0 | 0% |
| Customer_ID | 26 | 1.30% |
| Product | 7 | 0.35% |
| Category | 0 | 0% |
| Region | 16 | 0.80% |
| Quantity | 23 | 1.15% |
| Revenue | 27 | 1.35% |
| Profit | 29 | 1.45% |

The highest number of missing values occurs in the Profit column, followed by Customer_ID and Revenue.

## 4. Duplicate Records

A total of 23 duplicate rows were identified in the raw dataset.

Duplicate records can cause transactions to be counted more than once and can affect totals, averages, and other analytical results.

## 5. Inconsistent Categories

Inconsistent capitalization was identified in categorical columns.

### Category

The following variations were found:

- Electronics / electronics / ELECTRONICS
- Furniture / furniture / FURNITURE
- Home / home / HOME
- Beauty / beauty / BEAUTY
- Apparel / apparel / APPAREL

### Region

The following capitalization variations were found:

- Delhi / delhi / DELHI
- Mumbai / mumbai / MUMBAI
- Bangalore / bangalore / BANGALORE
- Chennai / chennai / CHENNAI
- Kolkata / kolkata / KOLKATA
- Hyderabad / hyderabad / HYDERABAD
- Pune / pune / PUNE

These values should be standardized before analysis.

## 6. Incorrect Dates

The `Order_Date` column contains 24 invalid or suspicious date entries.

Examples include:

- 31-02-2026
- 31-09-2026
- 00-06-2026
- 31-04-2026
- 29-02-2026
- 30-02-2026
- 31-06-2026
- 31-11-2026

These dates do not represent valid calendar dates and require investigation before time-based analysis.

## 7. Formatting Problems

The `Revenue` column contains inconsistent monetary representations.

Examples include:

- Numeric values such as `50000`
- Values containing `INR`, such as `374814 INR`
- Values containing currency symbols
- Encoding-affected values such as `â‚¹50000`
- Values containing comma formatting

A total of 323 non-standard revenue-format entries were identified.

The Revenue column should be converted into a consistent numerical format before calculations are performed.

## 8. Unusual Values

### Negative Quantity

A total of 41 records contain negative quantities.

Negative quantities should be investigated because they may represent data-entry errors or another business meaning that needs confirmation.

### Negative Profit

A total of 15 records contain negative profit values.

Negative profit is not automatically an error because it may represent a loss-making transaction. These records should therefore be investigated rather than automatically removed.

### Statistical Outliers

Using the IQR method:

| Column | Outliers |
|---|---:|
| Quantity | 19 |
| Revenue | 234 |
| Profit | 188 |

Outliers should be investigated before deciding whether they are genuine business values or data-quality problems.

## 9. Data Quality Summary

| Issue | Finding |
|---|---:|
| Total Rows | 2,000 |
| Missing Customer_ID | 26 |
| Missing Product | 7 |
| Missing Region | 16 |
| Missing Quantity | 23 |
| Missing Revenue | 27 |
| Missing Profit | 29 |
| Duplicate Rows | 23 |
| Invalid/Suspicious Dates | 24 |
| Non-standard Revenue Formats | 323 |
| Negative Quantities | 41 |
| Negative Profits | 15 |

## 10. Recommended Cleaning Actions

The identified issues should be handled carefully:

- Investigate and appropriately handle missing values.
- Remove or resolve duplicate records after verification.
- Standardize Category and Region values.
- Correct or handle invalid dates.
- Convert Revenue into a consistent numerical format.
- Investigate negative quantities before deciding whether they are errors.
- Investigate statistical outliers rather than deleting them automatically.
- Preserve legitimate negative-profit transactions because they may represent genuine business losses.

## 11. Masterclass 1 Principle

The Masterclass recommends an AI-assisted cleaning workflow:

Ask AI → Review → Verify → Apply

AI can suggest possible solutions, but the analyst is responsible for checking whether the solution is correct.

## 12. Conclusion

The raw dataset contains multiple data-quality issues that must be addressed before it can be considered analysis-ready.

The next stage is to apply appropriate cleaning and create a reliable dataset for further analysis.
