# UrbanStyle Customer Data Cleaning

## Overview

This project focuses on cleaning and preparing customer data using
Python and pandas. The dataset contains common data quality issues such
as missing values, inconsistent formats, and duplicates.

The script walks through a full data cleaning pipeline and produces a
structured dataset ready for analysis.

## Technologies Used

-   Python
-   pandas
-   numpy

## Features

### Data Loading and Exploration

-   Loads dataset from a simulated CSV file
-   Displays initial structure and data types
-   Identifies missing values and duplicate records

### Missing Data Handling

-   Fills missing satisfaction ratings with median values
-   Uses forward fill for missing purchase dates
-   Replaces missing names, phone numbers, and loyalty status
-   Fills missing age values with median

### Data Type Correction

-   Converts date columns into datetime format
-   Cleans currency values and converts to numeric
-   Ensures numeric consistency across relevant columns

### Text Standardization

-   Formats names into proper case
-   Standardizes category labels
-   Cleans and formats phone numbers into XXX-XXX-XXXX format

### Duplicate Removal

-   Identifies duplicate records
-   Removes duplicates while keeping the first occurrence

### Feature Engineering

-   Calculates days since last purchase
-   Computes average purchase value per customer
-   Classifies customers into purchase frequency groups:
    -   High
    -   Medium
    -   Low

### Data Cleanup

-   Renames columns for clarity
-   Removes unnecessary columns such as email
-   Sorts customers by total spending

### Insights Generation

-   Average spending by loyalty status
-   Revenue by product category
-   Correlation between satisfaction rating and spending

## How to Run

1.  Install required libraries: pip install pandas numpy

2.  Run the script: python your_script_name.py

3.  Review the printed report and cleaned dataset preview.

## Output

The script prints: - Data quality issues summary - Standardization steps
applied - Key business insights - Preview of cleaned dataset

## Key Insights

-   Customer spending varies by loyalty tier
-   Certain product categories generate higher revenue
-   Satisfaction rating shows a measurable relationship with spending

## Notes

-   The dataset is simulated using StringIO
-   No external files are required
-   The script runs end-to-end without manual input

## Author

Justin Dixon
