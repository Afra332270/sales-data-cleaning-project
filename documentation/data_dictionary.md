A data dictionary is a simple rulebook which includes includes basic description of each column. It gives an idea about what each column represents, the valid data type required for each column attribute, and the range of values that are valid for each attribute. The table below represents the data dictionary for this sales dataset.

| Column | Data Type | Description | Required | Unique | Example | Constraints | Nullable | Source | Notes |
|---|---|---|---|---|---|---|---|---|---|
| Transaction_ID | Text | Unique identifier for each transaction | Yes | Yes | T0001 | Must be unique | No | Sales data | Primary key |
| Customer_ID | Text | Unique identifier for each customer making the transaction | Yes | No | C0012 | Must exist in Customers table | No | Sales data | Foreign key |
| Customer_Name | Text | Name of the customer | Yes | No | Rahim | Must be present | No | Sales data | — |
| City | Text | Customer's city | Yes | No | Dhaka | Standardized city name | No | Sales data | — |
| Product | Text | Product purchased | Yes | No | Laptop | Must exist in Products table | No | Sales data | Foreign key |
