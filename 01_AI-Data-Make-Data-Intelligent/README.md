# Masterclass 1 — AI + Data: Make Data Intelligent

## Overview

This folder contains the practical work completed for Masterclass 1 — AI + Data: Make Data Intelligent as part of the AICTE | IBM SkillsBuild Data Analytics with AI Internship Program 2026.

The objective of this Masterclass is to understand raw e-commerce data, identify data-quality problems, create a cleaner analysis-ready dataset, perform basic customer segmentation, and develop meaningful business questions.

## Masterclass Workflow

The practical workflow followed in this Masterclass is:

Raw Data → Clean Data → Business Questions

The work completed in this folder prepares the dataset for further analysis and decision-making.

## 1. Dataset Understanding

The practice dataset is an e-commerce transaction dataset containing information about:

- Orders
- Customers
- Products
- Categories
- Regions
- Quantity
- Revenue
- Profit

The dataset contains 2,000 rows and 9 columns in the original `Raw_Data` sheet.

Detailed dataset analysis is documented in:

`01_Dataset-Understanding/Dataset-Analysis.md`

## 2. Data Quality Analysis

The raw dataset was examined for common data-quality problems, including:

- Missing values
- Duplicate records
- Inconsistent categories
- Incorrect dates
- Revenue formatting problems
- Negative quantities
- Negative profits
- Statistical outliers

A total of 23 duplicate rows were identified.

Detailed findings are documented in:

`02_Data-Quality-Analysis/Data-Quality-Report.md`

## 3. Data Cleaning

A cleaned version of the dataset was created while preserving the original raw data.

The cleaning process included:

- Removing exact duplicate rows
- Standardizing Category values
- Standardizing Region values
- Cleaning Revenue formatting
- Validating Order_Date
- Flagging invalid dates
- Flagging negative quantities
- Flagging negative profits
- Preserving missing values for further investigation

The cleaned dataset contains 1,977 rows after duplicate removal.

The cleaning process is documented in:

`02_Data-Quality-Analysis/Cleaning-Log.md`

## 4. Customer Segmentation

A `Customer_Segment` field was added to the cleaned dataset.

Customers were classified as:

- `New Customer`
- `Repeat Customer`
- `Unknown Customer`

The segmentation logic is based on the number of transactions associated with each Customer_ID.

Detailed documentation:

`03_Customer-Segmentation/Customer-Segmentation.md`

## 5. Business Questions

Business questions were developed across four major areas:

- Sales
- Product
- Customer
- Region

The questions focus on measurable business problems such as revenue trends, product profitability, customer value, and regional performance.

Five priority questions were selected based on business impact.

Detailed questions are documented in:

`04_Business-Questions/Business-Questions.md`

## 6. Practice Dataset

The original practice dataset and cleaned dataset are stored in:

`05_Practice-Dataset/`

### Files

- `AI + Data_ Make Data Intelligent _ Masterclass 1 _ Practice Dataset.xlsx`
- `Cleaned_Dataset.xlsx`

The original dataset is preserved so that the cleaning process remains traceable.

## 7. Key Outcome

The main outcome of Masterclass 1 is the transformation of raw e-commerce data into a more consistent and analysis-ready dataset.

The completed workflow is:

Raw Data → Data Quality Analysis → Cleaned Data → Customer Segmentation → Business Questions

## 8. Masterclass Principle

The Masterclass follows the AI-assisted data-cleaning approach:

Ask AI → Review → Verify → Apply

AI can suggest possible solutions, but the analyst must review and verify the results before applying them.

## 9. Skills Practiced

Through this Masterclass, the following skills were practiced:

- Dataset understanding
- Data-quality analysis
- Data cleaning
- Data standardization
- Date validation
- Revenue formatting
- Customer segmentation
- Business-question formulation
- Analytical thinking
- AI-assisted data analysis

