# Lending Club Case Study

## Table of Contents
* [Project Info](#project-info)
* [Objectives](#objectives)
* [Data Cleaning](#data-cleaning)
* [Analysis](#analysis)
* [Technologies Used](#technologies-used)
* [Contact](#contact)


## Project Info
Lending Club, a consumer finance company, provides various types of loans to urban customers.
Upon receiving a loan application, the company evaluates the applicant's profile to decide on approval or rejection. The challenge is to identify key factors influencing this decision and mitigate financial losses caused by loan defaults.


## Objectives
The primary goal is to analyze the dataset provided by Lending Club to:
- Identify variables that are strong indicators of loan defaults.
- Understand patterns in customer and loan attributes to optimize loan approval decisions.


## Data Cleaning
- Removed Whitespace: Strip any extra whitespace from column names or string values.
- Duplicate Dropped: Drop duplicate rows from the dataset.
- Data Type Conversion: Convert columns to appropriate data types (e.g., integers, floats, categories).
-  Handle Missing Values: Use mean, median, or mode to fill missing values based on the column's characteristics.
- Drop columns with more than 90% missing values.
- Formatted Columns: Apply formatting to columns if necessary (e.g., dates, currency)


## Analysis
- Loan Amount & Interest Rates: Higher values correlate with increased default risk.
- Annual Income & DTI: Lower income and higher DTI ratios indicate financial strain and default likelihood.
- Loan Grades: Lower grades (D-G) show higher default rates.
- Loan Terms: 36-month terms have a higher proportion of fully paid loans.
- Home Ownership: Renters and those with mortgages are more prone to defaults.
Refer to the report and code for detailed analysis and recommendations.


## Technologies Used
- Anaconda - Version 2.6.3
- Jupyter Notebook - Version 7.2.2
- pandas - Version 2.2.2
- numpy - Version 1.26.4
- matplotlib - Version 3.9.2
- seaborn - Version 0.13.2


## Contact
Created by:
* [Lekhana Gowda](https://github.com/LekhanaBC)
* [Jayant Lohani](https://github.com/JLohani)
