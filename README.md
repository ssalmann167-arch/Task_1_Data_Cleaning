Marketing Campaign Data Cleaning

Project Overview

This project focuses on cleaning and preprocessing a marketing campaign dataset. The main objective is to identify and handle data quality issues and prepare the dataset for further analysis and machine learning applications.

Dataset Information

- Dataset Type: Marketing Campaign / Customer Data
- Number of Rows: 2,240
- Number of Columns: 29
- Date Column: "Dt_Customer"
- Date Range: 2012-07-30 to 2014-06-29

Data Cleaning Steps

The following data cleaning and preprocessing steps were performed:

1. Loaded the marketing campaign dataset using Pandas.
2. Checked the dataset structure and data types.
3. Identified missing values.
4. Checked and removed duplicate records.
5. Converted the customer date column into the appropriate date format.
6. Performed outlier analysis on income values using the IQR method.
7. Identified potential income outliers.
8. Retained the potential income outliers because there was no sufficient evidence that the values were incorrect.
9. Exported the cleaned dataset as "cleaned_marketing_campaign.csv".

Outlier Analysis

The Income column was analyzed using the Interquartile Range (IQR) method.

- IQR: 32,751.00
- Upper Bound: 117,416.25
- Potential Outliers Identified: 8
- Income Outliers Removed: 0

The identified outliers were retained because high-income values can represent legitimate customers, and there was no evidence that these records were incorrect.

Final Data Quality

After cleaning:

- Rows: 2,240
- Columns: 29
- Missing Values: 0
- Duplicate Rows: 0
- Potential Income Outliers: 8
- Income Outliers Removed: 0

Files in This Repository

- "marketing_campaign.csv" — Original dataset
- "cleaned_marketing_campaign.csv" — Cleaned dataset
- "task_1_data_cleaning.ipynb" — Jupyter Notebook containing the cleaning process
- "README.md" — Project documentation

Tools Used

- Python
- Pandas
- Jupyter Notebook
- Visual Studio Code
- Git
- GitHub

Conclusion

The marketing campaign dataset was successfully cleaned and prepared for further analysis. Missing values and duplicate records were addressed, dates were processed appropriately, and potential income outliers were analyzed using the IQR method.

The final dataset contains 2,240 rows and 29 columns with no missing values or duplicate records.

---

Project: Marketing Campaign Data Cleaning
Status: Completed
