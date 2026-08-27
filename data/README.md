# Marketing Campaign Data Cleaning

## Project Overview

This project focuses on cleaning and preprocessing a marketing campaign dataset. The dataset contains 2,240 customer records and 29 columns.

The main objective of this project is to clean the dataset and make it ready for further analysis and visualization.

## Dataset Information

* **Number of rows:** 2,240
* **Number of columns:** 29
* **Dataset type:** Marketing campaign/customer data
* **Date column:** `dt_customer`

## Data Cleaning Steps

The following data-cleaning steps were performed:

1. Loaded the marketing campaign dataset using Python and Pandas.
2. Standardized the column names.
3. Checked for missing values.
4. Filled missing values in the `income` column using the median.
5. Checked for duplicate rows.
6. Standardized text values.
7. Converted the `dt_customer` column to the correct datetime format.
8. Checked and verified the data types of all columns.
9. Identified potential outliers in the `income` column using the IQR method.
10. Retained the identified outliers because they were not confirmed to be data-entry errors.
11. Performed a final data-quality check.

## Outlier Analysis

The IQR method was used to identify potential outliers in the `income` column.

* **Q1:** 35,538.75
* **Q3:** 68,289.75
* **IQR:** 32,751.00
* **Upper bound:** 117,416.25
* **Potential outliers identified:** 8

The outliers were retained because high-income values can represent legitimate customers and there was no evidence that these records were incorrect.

## Final Data Quality

After cleaning:

* **Rows:** 2,240
* **Columns:** 29
* **Missing values:** 0
* **Duplicate rows:** 0
* **Potential income outliers:** 8
* **Income outliers removed:** 0
* **Date range:** 2012-07-30 to 2014-06-29

## Tools Used

* Python
* Pandas
* VS Code
* Git
* GitHub

## Project Files

* `cleaned_marketing_campaign.csv` — Cleaned dataset
* `README.md` — Project documentation
* `data_cleaning.py` — Python data-cleaning code

## Conclusion

The marketing campaign dataset was successfully cleaned and validated. Missing values, duplicates, inconsistent formatting, date formatting, data types, and potential outliers were checked and handled appropriately.

The final cleaned dataset contains 2,240 rows and 29 columns with no missing values or duplicate records and is ready for further analysis.
