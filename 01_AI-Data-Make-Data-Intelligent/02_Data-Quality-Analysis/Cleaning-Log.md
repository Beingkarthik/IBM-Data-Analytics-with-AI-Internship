# Data Cleaning Log

## 1. Objective

The objective of this cleaning process was to transform the raw e-commerce dataset into a more consistent, analysis-ready dataset while preserving the original raw data.

The original `Raw_Data` sheet was not modified.

## 2. Input Dataset

- Original rows: 2,000
- Original columns: 9
- Source sheet: `Raw_Data`

## 3. Cleaning Operations Performed

### 3.1 Duplicate Records

- Exact duplicate rows identified: 23
- Duplicate rows removed: 23
- Rows remaining after duplicate removal: 1,977

### 3.2 Category Standardization

The `Category` column was standardized so that different capitalization styles represent the same category.

Examples:

- `Electronics`
- `electronics`
- `ELECTRONICS`

were standardized to:

`Electronics`

Similar standardization was applied to other categories.

### 3.3 Region Standardization

The `Region` column was standardized using consistent capitalization.

Examples:

- `Delhi`
- `delhi`
- `DELHI`

were standardized to:

`Delhi`

The same approach was applied to the other regions.

### 3.4 Revenue Cleaning

The `Revenue` column contained different monetary representations.

Examples included:

- Numeric values
- Currency symbols
- `INR` text
- Comma formatting
- Encoding-affected currency symbols

These representations were converted into a consistent numerical format.

### 3.5 Date Validation

The `Order_Date` column was converted to a consistent date format.

Invalid calendar dates were converted to blank values and flagged for review rather than being silently replaced with guessed dates.

### 3.6 Negative Quantities

Negative quantities were not automatically deleted.

They were preserved and flagged because they may represent data-entry problems or another business meaning that requires investigation.

### 3.7 Negative Profit

Negative profit values were preserved.

A negative profit may represent a genuine loss-making transaction and therefore should not automatically be treated as an error.

### 3.8 Missing Values

Missing values were not blindly filled with guessed values.

They remain available for further investigation and appropriate handling during later analysis.

## 4. Enrichment

The cleaned dataset was extended with analytical fields:

- `Month`
- `Year`
- `Customer_Segment`

### Customer Segment

Customers were classified based on the number of transactions:

- `New Customer` — customer appears once
- `Repeat Customer` — customer appears more than once
- `Unknown Customer` — Customer_ID is missing

## 5. Output Dataset

The cleaned workbook is:

`Cleaned_Dataset.xlsx`

It contains:

### `Cleaned_Data`

The cleaned and enriched dataset.

### `Cleaning_Summary`

A summary of the cleaning operations and important data-quality observations.

## 6. Verification

The cleaned dataset was checked after the cleaning operations.

The original raw dataset was preserved separately so that the cleaning process remains traceable.

## 7. Cleaning Principle

The cleaning process follows the Masterclass 1 approach:

Ask AI → Review → Verify → Apply

AI can suggest possible cleaning actions, but the analyst must review and verify the results before applying them.

## 8. Result

The raw dataset was transformed from 2,000 rows to 1,977 rows after removing 23 exact duplicate rows.

The cleaned dataset is now prepared for the next stage of analysis and enrichment.

