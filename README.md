## Project overview
The goal of this project is to demonstrate the sequence of data cleaning steps required to effectively clean and standardize a dataset for further use and analysis.
The project covers dataset preparation, data quality assessment, data cleaning, and documentation of the cleaning process. For this project, I have created both a clean and messy version of the dataset, and have ensured that the dataset has the right properties for it to be as close as possible to a real-world sales dataset. 

## Dataset overview
The dataset has 300 rows and 10 columns. Each row represents information of each transaction, while each column represents each attribute related to the transaction information. The columns are:  
- Transaction_ID
- Customer_ID
- Customer_Name
- City
- Product
- Quantity
- Unit_Price
- Total_Amount
- Payment_Method

Two versions of the dataset are included:
- sales_clean.csv : The original, clean dataset containing no errors.
- sales_messy.csv : The messy version of the dataset.

The files can be found in the [data folder] (data/).

## Data Dictionary
More information on the attributes of the dataset, such as what each column represents can be found in the data_dictionary.md

## Data Quality Rules
A set of data quality rules have been defined for the dataset to follow, to identify potential issues and ensure that the dataset meets accepted standards. The rules cover criteria about completeness, uniqueness, validity, accuracy and integrity of values in the dataset. More on the rules can be found here.

## Dataset Preparation
Detailed description on how the original, clean version of the dataset (sales_clean.csv) was created and how the messy version (sales_messy.csv) was created can be found in the ... file.

## Data Cleaning Process
Before starting the cleaning process, I first decide to take a systematic approach and perform data profiling on the dataset to better understand its structure, and find out if the dataset meets accepted standards (such as completeness, uniqueness, consistency, etc.). To do so, I take on some data profiling questions and try to answer them on the basis of this dataset. The questions include:

### <ins>Dataset Structure</ins>

- How many rows and columns are present in the dataset?
- What does one row represent?
- What is the expected grain of the dataset?
- Which column should uniquely identify each transaction?
- Are all the columns using the correct data types?

### <ins>Completeness</ins>

- Are there any completely blank rows?
- Are there any "NULL", "N/A", "-", "Unknown" fields?
- Are any required fields blank?

### <ins>Duplicates and Uniqueness</ins>

- Are there any duplicate Transaction_IDs?
- Are there any exact duplicate Transaction_IDs?
- Are there any duplicate Transaction_IDs with different information?

### <ins>Referential Integrity</ins>

- Does every Customer_ID exist in the Customers reference table?
- Does every Customer_Name, City correspond to the correct Customer_ID?
- Are there any exact duplicate Customer_IDs with the same information?
- Does every Product name exist in the Products reference table?
- Does every Product have the correct Unit_Price?
- Does every Payment_Method name exist in the Payments reference table?


### <ins>Numerical Accuracy</ins>

- Does every Unit_Price and every Total_Amount value follow the right constraints?
- Does every Quantity value follow the right contraints?
- Is every Total_Amount value calculated correctly using the correct formula (Quantity * Unit_Price)?
- Do all the numerical values consistently follow the correct format and correct datatype throughout the dataset?


### <ins>Date Validity</ins>

- Does every Last_Updated value follow the right constraints?
- Are all the Last_Updated values valid dates following the correct data type?
- Are all the dates stored consistently?

### <ins>Consistency</ins>

- Do all the Transaction_ID values follow the correct format consistently throughout the dataset?
- Do all the Customer_ID values follow the correct format consistently throughout the dataset?
- Do all the Last_Updated values follow the correct format consistently throughout the dataset?
- Do all the numerical values follow the correct format consistently throughout the dataset?
- Do all the categorical values follow the correct format consistently throughout the dataset?
  












