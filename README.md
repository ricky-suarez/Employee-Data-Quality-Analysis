# Employee Data Quality Analysis

## Overview

This project focuses on assessing, cleaning, transforming, and merging employee data using Python and Pandas. The goal was to identify data quality issues and prepare multiple datasets for accurate analysis.

The project demonstrates practical skills in data profiling, data cleaning, data transformation, anomaly detection, and dataset integration.

## Technologies Used

- Python
- Pandas
- Jupyter Notebook
- Data Profiling
- Data Cleaning
- Data Transformation
- Data Validation

## Project Objectives

The main objectives of the project were to:

- Profile employee datasets to understand their structure and quality
- Identify missing, incorrect, or unusual values
- Detect invalid age values and other data anomalies
- Standardize employee information between datasets
- Transform employee names into consistent fields
- Merge multiple datasets using common employee information
- Verify that the final merged dataset was accurate and complete

## Data Cleaning and Profiling

The datasets were reviewed using Pandas to identify potential data quality problems.

Examples of issues examined included:

- Missing values
- Incorrect data types
- Duplicate or inconsistent records
- Negative age values
- Unrealistically high age values
- Formatting differences between datasets

Data profiling helped determine which records required additional review or cleaning before the datasets could be combined.

## Data Transformation

One dataset stored employee names in a single `Employee_Name` column, while another dataset stored names separately.

The employee name data was transformed into:

- `First_Name`
- `Last_Name`

This allowed both datasets to use a consistent structure before merging.

## Dataset Merge

The datasets were combined using a left merge based on the following fields:

```python
["First_Name", "Last_Name", "DOB"]
