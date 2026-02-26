# Project Overview
An end-to-end data analysis project examining 50,000+ retail transactions from the Global Superstore dataset. Using advanced Excel techniques, this project explores sales patterns, pricing strategies, product performance, and operational efficiency across 147 countries and 15 years of business operations.

Linkedin Post: https://www.linkedin.com/in/paul-gikonyo-15389418b?miniProfileUrn=urn%253Ali%253Afsd_profile%253AACoAACzNhM8B6HD_yIkGpHSdjRGHqGPBsClH7fs&skipRedirect=true&miniProfileUrn=urn%3Ali%3Afsd_profile%3AACoAACzNhM8B6HD_yIkGpHSdjRGHqGPBsClH7fs

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

Rank	Country	Sales Revenue	
1. United States	
2. Australia
3. France
4. China
5. Germany

Insight: Developed markets (US, Europe) dominate revenue, while emerging markets show growth potential.

Top 5 Most Profitable Sub-Categories (All Time):
1.	Copiers
2.	Phones
3.	Accessories
4.	Paper
5.	Binders
   
Insights:
•	Technology products consistently top profitability rankings
•	Furniture shows high revenue but lower margins (bulky shipping costs)
•	Office supplies provide steady, predictable cash flow

Product Price varying with Sales

Unit Price vs. Sales Volume Analysis:
• Correlation Coefficient: -0.89 -> negative correlation

•	Finding: Generally, lower-priced items sell in higher volumes

•	Exception: Premium technology products (smartphones, laptops) maintain high prices with strong demand

Identified Two Market Segments:
1.	Volume Market: Low unit price ($5-$50), high quantity (office supplies, accessories)
2.	Premium Market: High unit price ($200-$2,000), moderate quantity (copiers, phones)

Percentage Delivery across countries

Key Findings:
•	Moderate discounts (10-20%) increase transaction size without destroying margins
•	Heavy discounts (>30%) often indicate clearance or end-of-life products
•	No-discount sales have highest profit margins but lower average order value
•	Sweet spot: 10-15% discount for optimal revenue-profit balance

# Technical Implementation
Excel Features Utilized
Advanced Formulas:
LOOKUP Functions: VLOOKUP, XLOOKUP, INDEX-MATCH

Conditional Aggregation: SUMIFS, COUNTIFS, AVERAGEIFS, MAXIFS

Text Functions: TRIM, PROPER, LEFT, RIGHT, CONCATENATE, TEXTJOIN

Date Functions: YEAR, MONTH, EOMONTH, DATEVALUE, WEEKDAY

Logical: IF, IFS, AND, OR, nested conditionals

Statistical: AVERAGE, MEDIAN, STDEV, CORREL, PERCENTILE

# Prerequisites
- Microsoft Excel 2019
- Basic understanding of Excel formulas and pivot tables

#Getting Started
1. **Download the dataset:**

   Visit: https://www.kaggle.com/datasets/apoorvaappz/global-super-store-dataset
   Download: Global_Superstore2.csv or .xlsx
2. **Clone this repository:**
bash
   git clone https://github.com/Chege-jr0/Global-SuperStore-Analysis.git

3. **Open the analysis files:**
   - Start with `Global_Superstore_Cleaned.xlsx` for processed data

4. **Recreate the analysis:**
   - Customize dashboards based on your interests

# Skills Demonstrated

✅ Advanced Excel proficiency (formulas, pivot tables, dashboards)  
✅ Data cleaning and transformation techniques  
✅ Exploratory data analysis (EDA)  
✅ Statistical analysis and correlation studies  
✅ Business intelligence and data visualization  
✅ Insight generation and storytelling with data  
✅ Dashboard design and interactive reporting  




