### Data Quality Report
This report presents the number of data quality issues that were found during the data profiling stage of the data cleaning process. All the findings are summarized
below:

### Dataset structure:

| Metric | Result |
| --- | --- |
| Rows examined | 313 |
| Expected transaction rows | 299 |
| Columns | 10 |
| Date range | 2009-2035 |
| Reference tables | Customers, Products, Cities |

## 3. Data Quality Assessment

### 3.1 Completeness

| Column | Missing Values | Notes |
| --- | ---: | --- |
| Transaction_ID | 0 | Pass |
| Customer_ID | 0 | Pass |
| Customer_Name | 4 | Fail |
| City | 3 | Fail |
| Product | 0 | Pass |
| Quantity | 2 | Fail |
| Unit_Price | 1 | Fail |
| Total_Amount | 4 | Fail |
| Payment_Method | 5 | Fail |
| Last_Updated | 2 | Fail |


### 3.2 Uniqueness

| Column | Duplicate Values | Notes |
| --- | ---: | --- |
| Transaction_ID | 0 | Pass |
| Customer_ID | 0 | Pass |
| Customer_Name | 4 | Fail |
| City | 3 | Fail |
| Product | 0 | Pass |
| Quantity | 2 | Fail |
| Unit_Price | 1 | Fail |
| Total_Amount | 4 | Fail |
| Payment_Method | 5 | Fail |
| Last_Updated | 2 | Fail |


### 3.3 Validity

| Issue | Column | Findings | Notes |
| --- | ---: | --- | --- |
| Incorrect data type | Transaction_ID | Pass | check |
| Incorrect data type | Transaction_ID | Pass | check |
| Incorrect format | Transaction_ID | Pass | check |
| Text inconsistencies | Transaction_ID | Pass | check |


### 3.4 Accuracy

| Check | Findings | Notes | 
| --- | ---: | --- |
| Unit_Price>0 | Transaction_ID | Pass | 
| Incorrect data type | Transaction_ID | Pass | 
| Incorrect format | Transaction_ID | Pass | 
| Text inconsistencies | Transaction_ID | Pass | 


### 3.5 Referential integrity

| Column -> Reference column/table | Findings | Notes |
| --- | ---: | --- |
| Incorrect data type | Transaction_ID | Pass | 
| Incorrect data type | Transaction_ID | Pass | 
| Incorrect format | Transaction_ID | Pass | 
| Text inconsistencies | Transaction_ID | Pass | 







| Column(s) | Rule_ID | Category | Findings | Notes |
|---|---|---|---|---|
| All columns | DQ001 | Completeness | All required fields must contain a non-blank value. | |
| All columns | DQ013 | Accuracy | All required fields must follow the correct data type. | |
| All columns | DQ018 | Consistency | All required fields must contain a non-blank value. | |
| All columns | DQ019 | Consistency | All required fields must contain a non-blank value. | |
| All columns | DQ021 | Null value consistency | All required fields must contain a non-blank value. | |
| All rows | DQ022 | Record Integrity | All required fields must contain a non-blank value. | |
| All columns | DQ023 | Multi-rule validation | All required fields must contain a non-blank value. | |
