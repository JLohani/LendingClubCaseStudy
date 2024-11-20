# Lending Club Case Study

## Table of Contents
* [Problem Statement](#problem-statement)
* [Objectives](#objectives)
* [Data Cleaning](#data-cleaning)
* [EDA_Analysis](#eda-analysis)
* [Observations](#observations)
* [Technologies Used](#technologies-used)
* [Contact](#contact)


## Problem Statement
We work for a consumer finance company which specialises in lending various types of loans to urban customers. 
When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. 
Two types of risks are associated with the bank’s decision:
- If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company
- If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company

When a person applies for a loan, there are two types of decisions that could be taken by the company:
- Loan accepted: If the company approves the loan, there are 3 possible scenarios described below:
    - Fully paid: Applicant has fully paid the loan (the principal and the interest rate)
    - Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.
    - Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan 

- Loan rejected: The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)


## Objectives
The company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface. 
Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'.
The company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default. The company can utilise this knowledge for its portfolio and risk assessment.
In this case study, we will use EDA to understand how consumer attributes and loan attributes influence the tendency of default.


## Data Cleaning
- Removed Whitespace: Strip any extra whitespace from column names or string values.
- Duplicate Dropped: Drop duplicate rows from the dataset.
- Data Type Conversion: Convert columns to appropriate data types (e.g., integers, floats, categories).
-  Handle Missing Values: Use mean, median, or mode to fill missing values based on the column's characteristics.
- Drop columns with more than 90% missing values.
- Formatted Columns: Apply formatting to columns if necessary (e.g., dates, currency)

## EDA Analysis
- Univariate Analysis
  - A majority of loan amounts are clustered around $5,000 to $15,000.
  - A small number of borrowers have very high incomes, which might represent outliers extending the range beyond $500,000.
  - Few borrowers have a DTI ratio above 30%, which could indicate better financial stability for the majority.
  - Lenders naturally prioritize issuing loans to higher subgrade A and B.
  - The majority of borrowers either rent their homes or have a mortgage indicating potential financial obligations., and few have their own house

- Bivariate Analysis
  - Outliers in the "Charged Off" category indicate that even larger loans have defaulted occasionally.
  - The median loan amount for "Charged Off" loans is slightly higher than that for "Fully Paid" loans.
  - Interest rates tend to be higher for Charged Off loans compared to Fully Paid loans, suggesting higher rates may correlate with loan defaults.
  - Borrowers with higher interest rates face a significantly higher risk of default, particularly for mid-to-large loan amounts.
  - Lenders should carefully assess the creditworthiness of applicants seeking loans with higher amounts and higher rates to reduce default rates.
  - Borrowers with lower interest rates are generally more reliable in loan repayment.


## Observations
- Higher loan amounts increase default risk.
- Higher interest rates correlate with higher default rates, especially for larger loans.
- Lower annual incomes are associated with a higher likelihood of default.
- Higher DTI ratios suggest financial strain, raising default risk.
- Lower loan grades (D, E, F, G) are significant indicators of higher default probability.
- Renters or those with mortgages may be more vulnerable to default due to other financial obligations.


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
