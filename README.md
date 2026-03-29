Sales Report Analysis

A data analytics project that analyzes sales data to identify key trends, track product performance, understand customer behavior, and provide actionable business insights using MySQL, Excel, and Power BI.

Power BIMySQLExcelLicense

Aim
To analyze sales data, identify key trends, and provide insights into product performance, customer behavior, and revenue growth. The project helps businesses make data-driven decisions for improving sales strategies.

Objective
Prepare and analyze sales data to track revenue
Identify top-performing products and regions
Generate actionable insights through data visualization
Support better business decision-making
Keywords
Sales Analysis Revenue Trends Customer Behavior Profit & Loss Product Performance Data Visualization Power BI Excel MySQL Business Insights Dashboard Reporting Decision Making

Tech Stack
Tool	Purpose
MySQL Community Server	Database creation and data storage
MySQL Workbench	Query execution and database management
Microsoft Excel	Data import, export, and formatting
Power BI	Data visualization and dashboard creation
 
 
 Project Structure

sales-report-analysis/  

├── database/
│ ├── schema.sql
│ ├── tables.sql
│ ├── data_insertion.sql
│ ├── queries/
│ │ ├── operators.sql
│ │ ├── aggregate_functions.sql
│ │ ├── clauses.sql
│ │ ├── joins.sql
│ │ └── case_statements.sql
│ └── sample_queries.sql
├── data/
│ ├── raw/
│ │ └── sales_data.xlsx
│ └── processed/
│ └── cleaned_sales.xlsx
├── power-bi/
│ ├── sales_dashboard.pbix
│ └── data_model.png
├── screenshots/
│ ├── database_tables.png
│ ├── power_bi_transform.png
│ ├── dashboard.png
│ └── dax_measures.png
├── README.md
└── LICENSE


## Prerequisites

- MySQL Community Server 8.0+
- MySQL Workbench
- Microsoft Excel (2016 or later)
- Power BI Desktop

## Installation

### 1. Set Up MySQL Database

```bash
# Login to MySQL
mysql -u root -p

# Create and use database
CREATE DATABASE sales_analysis;
USE sales_analysis;

# Run schema and tables
SOURCE database/schema.sql;
SOURCE database/tables.sql;
SOURCE database/data_insertion.sql;
. Import Data via Excel
Open data/raw/sales_data.xlsx in Excel
Clean and format the data
Export as data/processed/cleaned_sales.xlsx
Import into MySQL using MySQL Workbench
3. Connect Power BI
Open Power BI Desktop
Click Get Data → Database → MySQL database
Enter server credentials
Select sales_analysis database
Load data
4. Open Dashboard
Open power-bi/sales_dashboard.pbix
Click Refresh to update data
Procedure
Database Creation
Created the database and defined table structures in MySQL to store sales data including product details, customer information, order records, and regional data.

SQL Operations Performed
Operators Used
Operator
Description
=	Equal to
!=	Not equal to
>	Greater than
>=	Greater than or equal to
<	Less than
<=	Less than or equal to
IS NULL	Check for null values
IS NOT NULL	Check for non-null values
AND	Logical AND
OR	Logical OR
BETWEEN	Range filter
NOT BETWEEN	Exclude range
IN	Match from a list
NOT IN	Exclude from a list

Aggregate Functions
Function
Purpose
MIN()	Find minimum value
MAX()	Find maximum value
COUNT()	Count total records
SUM()	Calculate total sum
AVG()	Calculate average value

Clauses Used
HAVING — Filter grouped data
DISTINCT — Remove duplicates
GROUP BY — Group records
ORDER BY — Sort results
LIMIT — Restrict number of rows
OFFSET — Skip rows
LIKE — Pattern matching
CASE — Conditional logic (IF-ELSE)
Joins
CROSS JOIN — Cartesian product of tables

Power BI Operations
Data Cleaning & Transformation
Cleaned raw data after import
Renamed columns for consistency
Capitalized each word in text fields
Trimmed extra spaces from data
DAX Formulas Used

## Prerequisit
Total Sales = SUM(sales[total_amount])

Total Quantity = SUM(sales[quantity])

Total Average = AVERAGE(sales[total_amount])
Dashboard
Created an interactive dashboard with visualizations for sales trends, product performance, and regional distribution.

Conclusion
The sales report revealed important insights such as:

High-performing products identified for revenue focus
Regional sales distribution mapped for targeted strategies
Seasonal trends discovered for inventory planning
Customer purchase behavior analyzed for retention strategies
By visualizing and analyzing the data, the project highlights opportunities to increase revenue, optimize inventory, and improve overall sales performance.
