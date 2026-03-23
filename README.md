# customer_behaviour_analysis
End-to-end data analysis project exploring customer shopping behavior using Python, SQL, and Power BI to uncover spending patterns, customer segments, and business insights.

Customer Shopping Behavior Analysis
Project Overview

This project analyzes customer shopping behavior using transactional data from 3,900 purchases to uncover insights about spending patterns, customer segments, product preferences, and subscription behavior.

The objective is to transform raw transactional data into actionable business insights using a full analytics workflow involving Python, SQL, and Power BI.

This project demonstrates an end-to-end data analytics pipeline, from data cleaning and feature engineering to business analysis and dashboard visualization.

Tech Stack

Languages & Tools

Python
SQL (PostgreSQL)
Power BI
Jupyter Notebook

Python Libraries

Pandas
NumPy
Matplotlib
Dataset Summary
Total Records: 3,900 transactions
Total Columns: 18 features
Key Data Categories

Customer Demographics

Age
Gender
Location
Subscription Status

Purchase Information

Item Purchased
Product Category
Purchase Amount
Season
Size
Color

Shopping Behavior

Discount Applied
Promo Code Used
Previous Purchases
Frequency of Purchases
Review Rating
Shipping Type
Data Quality
37 missing values found in the Review Rating column.
Missing values were handled using median imputation per product category.
Project Workflow
1. Data Cleaning & Preparation (Python)

Performed initial exploration and cleaning using Pandas in Jupyter Notebook.

Key steps included:

Data loading and inspection using df.info() and df.describe()
Handling missing values in review_rating
Standardizing column names using snake_case
Removing redundant columns
Creating new analytical features
Feature Engineering

New features created:

age_group – categorized customers into age segments
purchase_frequency_days – calculated purchase frequency
Data Validation
Verified redundancy between discount_applied and promo_code_used
Removed promo_code_used after confirming duplication.
Database Integration

The cleaned dataset was loaded into PostgreSQL for structured business analysis using SQL queries.

This step simulates how analysts work with production databases instead of spreadsheets.

Business Analysis Using SQL

SQL queries were written to answer key business questions:

Revenue Insights
Revenue contribution by gender
Revenue contribution by age group
Customer Behavior
Identified high-spending customers who used discounts
Analyzed repeat buyers vs subscription likelihood
Product Insights
Top 5 products by average rating
Top 3 most purchased products per category
Products with highest percentage of discounted purchases
Sales Strategy
Comparison of Express vs Standard shipping spend
Revenue comparison between Subscribers vs Non-Subscribers
Customer Segmentation

Customers were segmented into:

New Customers
Returning Customers
Loyal Customers

based on purchase history.

Power BI Dashboard

An interactive Power BI dashboard was built to visualize insights for stakeholders.

Key Dashboard Metrics
Revenue by Gender
Revenue by Age Group
Customer Segments
Top Products by Category
Discount Impact on Sales
Subscriber vs Non-Subscriber Revenue

The dashboard allows business users to quickly explore customer behavior patterns.

Key Business Insights
Certain age groups contribute significantly more revenue
Subscribers show stronger purchase behavior
Express shipping customers tend to spend more
Some products rely heavily on discount-driven sales
Business Recommendations

Based on the analysis:

1. Boost Subscription Adoption

Offer exclusive benefits or loyalty perks.

2. Launch Loyalty Programs

Convert returning customers into loyal customers.

3. Optimize Discount Strategy

Focus discounts on products that benefit most from promotions.

4. Highlight High-Rated Products

Use them in marketing campaigns to improve conversion.

5. Target High-Value Customer Segments

Personalize marketing for high-spending age groups.


Repository Structure
Customer-Shopping-Behavior-Analysis
│
├── data
│   └── dataset.csv
│
├── notebooks
│   └── data_cleaning_analysis.ipynb
│
├── sql
│   └── business_queries.sql
│
├── dashboard
│   └── powerbi_dashboard.pbix
│
└── README.md
Skills Demonstrated
Data Cleaning & Preparation
Exploratory Data Analysis
Feature Engineering
SQL Business Analysis
Customer Segmentation
Data Visualization
Business Insight Generation
Dashboard Development
Author

Yash Girme
