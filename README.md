# Project Overview
An end-to-end data analysis project examining 50,000+ retail transactions from the Global Superstore dataset. Using advanced Excel techniques, this project explores sales patterns, pricing strategies, product performance, and operational efficiency across 147 countries and 15 years of business operations.

# Key Questions Explored
1. Which Countries haad the top sales?
2. What are the top 5 profit making product types on a yearly basis?
3. How is the product price varying with the sales - Is there any increase in sales with the decrease in price at a day-level?
4. What is the percentage delivery time across the countries?

# Project Objectives

•	Data Cleaning & Validation: Transform raw transactional data into analysis-ready format
•	Exploratory Data Analysis: Uncover sales patterns, trends, and business insights
•	Financial Analysis: Evaluate profitability, pricing strategies, and discount impacts
•	Operational Insights: Assess delivery performance and fulfillment efficiency
•	Interactive Dashboards: Create executive-ready visualizations for data-driven decision-making

# Key Attributes
•	Transaction: Row ID, Order ID, Order Date, Ship Date, Ship Mode, Order Priority
•	Customer: Customer ID, Customer Name, Segment
•	Location: Country, City, State, Postal Code, Market, Region
•	Product: Category, Sub-Category, Product Name
•	Financial: Sales, Quantity, Discount, Profit, Shipping Cost

# Data Cleaning Process
1. Initial Assessment
excel
Original rows: 51,290
Columns: 24
Data types: Mixed (text, numbers, dates)
Issues identified: Duplicates, missing values, formatting inconsistencies

2. Data Quality Issues Resolved
Duplicates
•	Identified using Row ID as unique identifier
•	Removed duplicate transactions
•	Verified legitimate repeat customer orders retained

3. Missing Values
•	Postal Code: Some missing 
•	State: Missing for non-US countries 
•	Critical fields (Sales, Profit, Quantity): Zero missing after validation

4. Date Format Issues
•	Converted Order Date and Ship Date from text to proper date format
•	Created separate Year, Month, Quarter columns for time-series analysis

5. Data Type Corrections
•	Standardized Sales, Profit, Quantity, Shipping Cost to numeric
•	Converted Discount from text percentages to decimal format

6. Text Standardization
•	Removed leading/trailing spaces using TRIM
•	Standardized country names for consistency
•	Applied consistent capitalization

7. Data Validation
•	Identified impossible dates (ship before order): Flagged for review
•	Detected negative quantities: Marked as potential returns or errors
•	Found zero-value sales: Investigated and documented
•	Flagged extreme discounts (>80%): Potential data quality issues

# Analysis and Findings
Top 5 Countries by Total Sales:
Rank	Country	Sales Revenue	% of Total
1	United States	$X.XX M	XX%
2	[Country]	$X.XX M	XX%
3	[Country]	$X.XX M	XX%
4	[Country]	$X.XX M	XX%
5	[Country]	$X.XX M	XX%
Insight: Developed markets (US, Europe) dominate revenue, while emerging markets show growth potential.


