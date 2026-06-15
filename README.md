E-commerce Revenue & KPI Analysis (Python + SQL + Power BI)
Project Overview

This project is an end-to-end E-commerce Data Analytics solution built using Python, SQL Server, and Power BI. The goal is to analyze transactional retail data to uncover key business insights related to revenue performance, customer behavior, and product trends.

The project simulates a real-world analytics workflow:

Data Cleaning (Python) → Data Modeling (SQL) → Business Intelligence Dashboard (Power BI)

Business Problem
E-commerce businesses generate massive transactional data but often lack structured insights into:

Revenue trends over time
Customer purchasing behavior
Top-performing products
Order value and basket size
Sales performance across countries
This project transforms raw retail transactions into actionable KPIs and an executive dashboard for strategic decision-making.

Tools Used
Python (Google Colab) – Data cleaning & feature engineering
Pandas & NumPy – Data preprocessing
SQL Server (SSMS) – Data modeling, cleaning & KPI queries
Power BI – Data modeling, DAX measures & dashboard visualization
GitHub – Portfolio documentation & version control
Dataset
Source: UCI Online Retail Dataset Contains transactional data including:

InvoiceNo
StockCode
Description
Quantity
UnitPrice
CustomerID
Country
InvoiceDate
Data Cleaning & Preprocessing (Python)
Key preprocessing steps performed in Google Colab:

Removed cancelled orders (negative Quantity)
Filtered invalid transactions (UnitPrice ≤ 0)
Engineered Revenue column
Handled missing CustomerID (analyzed impact before cleaning)
Created YearMonth feature for trend analysis
Exported cleaned dataset for SQL modeling
SQL Data Modeling
Data was imported into SQL Server and structured into a star schema model:

Fact Table

retail_full (transactions & revenue metrics)
Dimension Tables

customers_clean
products_clean
SQL Contributions in this Project:

Data cleaning in SQL
Key KPIs Calculated
Total Revenue: 10,666,684+
Total Orders: 19,960
Total Customers: 4,338
Average Order Value (AOV)
Average Basket Size
Purchase Frequency
Monthly Sales Growth
Top-Selling Products
Power BI Dashboard Features
Sales Analysis

Total Revenue KPI Card
Total Transactions
Total Customers
Average Order Value (AOV)
Total Revenue by Product
Total Revenue by Month
Total Revenue by Quarter
Total Revenue by Country
Customer Analysis

Purchase Frequency Analysis
Total Customer
Average Basket Size
Customer Contribution to Revenue
Active Customers by Month
Top Customers by Country
Product Analysis

Top 10 Products by Quantity
Total Revenue
Number of Products
Product Quantity
Total Orders
Data Modeling (Power BI)
Star Schema implemented
One-to-Many relationships:
DateTable → retail_full
customers_clean → retail_full
products_clean → retail_full
DAX measures used for dynamic KPI calculations
Proper DateTable for time intelligence
Key Insights from Analysis
Revenue shows strong growth toward Q4, indicating seasonal purchasing trends -A small percentage of customers contribute significantly to total revenue
High AOV suggests bulk purchasing behavior
Certain products dominate revenue contribution
Missing CustomerID accounted for ~16% of revenue, highlighting data quality impact
Portfolio Value & Skills Demonstrated

This project demonstrates:

End-to-End Data Analytics Workflow
Data Cleaning (Python)
SQL Data Modeling & Querying
KPI Design & Business Metrics
Power BI Dashboard Development
Star Schema Implementation
Data Storytelling for Business Decisions
KPI aggregation queries
View creation for analytics
Data validation and transformation
Dashboard Preview
image image image
How to Run This Project
Open the Python notebook in Google Colab for data preprocessing
Import the cleaned dataset into SQL Server
Run SQL scripts to create tables and views
Connect Power BI directly to SQL Server
Open the .pbix file to explore the interactive dashboard
✅ Hover on any chart    → See detailed tooltips

