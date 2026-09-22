A data dictionary is a simple rulebook which includes includes basic description of each column. It gives an idea about what each column represents, the valid data type required for each column attribute, and the range of values that are valid for each attribute. The table below represents the data dictionary for this sales dataset.

| Column | Data Type | Description | Required | Unique | Example | Constraints | Nullable | Source | Notes |
|---|---|---|---|---|---|---|---|---|---|
| Transaction_ID | Text | Unique identifier for each transaction | Yes | Yes | T0001 | Must be unique | No | Sales data | Primary key |
| Customer_ID | Text | Unique identifier for each customer making the transaction | Yes | No | C0012 | Must exist in Customers table | No | Sales data | Foreign key |
| Customer_Name | Text | Name of the customer | Yes | No | Rahim Ahmed | Must match Customer_ID | No | Sales data | — |
| City | Text | Customer's city | Yes | No | Dhaka | Must match Customer_ID | No | Sales data | — |
| Product | Text | Name of product purchased | Yes | No | Laptop | Must exist in Products table | No | Sales data | - |
| Quantity | Integer | Number of units purchased | Yes | No | 4 | Must be a positive integer | No | Sales data | - |
| Unit_Price | Decimal | Price of one unit | Yes | No | 200.0 | Must be greater than 0. Must match with given unit price in Products table| No | Sales data | - |
| Total_Amount | Decimal | Total transaction value | Yes | No | Laptop | Must be greater than 0 and equal to Quantity * Unit_Price | No | Sales data | - |
| Payment_Method | Text | Method of payment for each customer | Yes | No | bKash | Must exist in Payments table | No | Sales data | - |
| Last_Updated | Date | Date when transaction record was last updated | Yes | No | 3/4/2025 | Must be valid, consistent and fall within the intended dataset period | No | Sales data | - |





