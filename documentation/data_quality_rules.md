## Data Quality Rules
The following rules define the expected data quality requirements for our sales dataset. These rules have been used during data profiling, cleaning and post-cleaning validation steps.

| Rule_ID | Category | Column(s) | Data Quality Rule |
|---|---|---|---|
| DQ001 | Completeness | All columns | All required fields must contain a non-blank value. |
| DQ002 | Uniqueness | Transaction_ID | Each Transaction_ID must be unique. |
| DQ003 | Referential Integrity | Customer_ID | Every Customer_ID must exist in the Customers reference table. |
| DQ004 | Referential Integrity | Payment_Method | Every Payment_Method must exist in the Payments reference table. |
| DQ005 | Referential Integrity | Product | Every Product must exist in the Products reference table. |
| DQ006 | Validity | Transaction_ID | Each Transaction_ID must follow the correct format.|
| DQ007 | Validity | Customer_ID | Each Customer_ID must follow the correct format. |
| DQ008 | Validity | Quantity | Quantity must be a positive integer. |
| DQ009 | Validity | Unit_Price | Unit_Price must be a numeric value greater than or equal to 0 and must exist in the Products table. |
| DQ010 | Validity | Product, Payment_Method | Both fields must also exist in the approved reference tables. |
| DQ011 | Validity | Customer_Name, City | Both fields must also exist in the approved reference tables. |
| DQ012 | Validity | Last_Updated | Last_Updated must be a valid date within the intended 2025 period. |
| DQ013 | Accuracy | All columns | All columns must follow the correct data type. |
| DQ014 | Accuracy | Total_Amount | Total_Amount must equal Quantity × Unit_Price. |
| DQ015 | Consistency | Customer_ID, Customer_Name | Each Customer_Name must consistently correspond to the correct Customer_ID |
| DQ016 | Consistency | Customer_ID, City | Each City must consistently correspond to the correct Customer_ID |
| DQ017 | Consistency | Product, Unit_Price | Unit_Price should consistently correspond to the correct Product |
| DQ018 | Consistency | All columns | Data in each column should consistently follow the right format throughout the dataset. |
| DQ019 | Consistency | All columns | Data in each column should consistently follow the right constraints throughout the dataset. |
| DQ020 | Text-Quality | Customer_Name, City, Product, Payment_Method | Text values should consistently follow the right capitalization and spelling conventions. |
| DQ021 | Null value consistency | All columns | Values such as 'N/A', "NULL", "Unknown", "-", should be handled consistently. |
| DQ022 | Record Integrity | All columns | There should not be any completely blank rows. |
| DQ023 | Multi-rule validation | All columns | Records should follow all data quality rules post cleaning. |
| DQ024 | Timeline consistency | All columns | Data in all columns should be recent and up to date for accurate analysis. |



###| DQ009 | Cross-field consistency | All columns | Related columns should agree with each other and follow logical relationships. |
