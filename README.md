# Customer Behavior Data Analyst Portfolio Project
## Project Overview

This project analyzes customer shopping behavior using transactional data from 3,900 purchases across multiple product categories. The objective is to identify patterns in customer spending, product preferences, and subscription behavior to support data-driven business decisions.

The project integrates Python, PostgreSQL, SQL, and Power BI to perform data cleaning, database analysis, and visualization.

## Objectives

Analyze customer purchase patterns

Identify high-value customers and segments

Evaluate the impact of discounts and subscriptions

Determine top-performing products and categories

Generate business insights and recommendations

## Dataset Summary

Total Records: 3,900

Total Features: 18

Key Variables:

Customer demographics: age, gender, location

Transaction details: item purchased, category, purchase amount

Customer behavior: frequency of purchases, previous purchases

Marketing indicators: discount applied, subscription status

Customer feedback: review rating

Missing values in the review rating column were handled using category-wise median imputation.

## Tools and Technologies Used

Python (Pandas, NumPy)

PostgreSQL

SQL

Power BI

SQLAlchemy

pgAdmin

## Project Workflow
### 1. Data Cleaning and Preparation (Python)

Loaded dataset using pandas

Checked data types, missing values, and summary statistics

Converted columns to proper formats

Handled missing values in review_rating

Renamed columns to snake_case format

Created new features:

age_group

purchase_frequency_days

Loaded cleaned data into PostgreSQL database

### 2. Database Integration (PostgreSQL)

Used SQLAlchemy to connect Python with PostgreSQL and stored cleaned data into a relational table.

Example:

engine = create_engine("postgresql+psycopg2://postgres:password@localhost:5432/customer_behavior")
df.to_sql("customer", engine, if_exists="replace", index=False)

### 3. SQL Analysis

Performed business-focused SQL queries including:

Revenue by gender

Top rated products

Customer segmentation (New, Returning, Loyal)

Discount effectiveness analysis

Subscription vs non-subscription analysis

Revenue by age group

Shipping type impact on spending

### Connect the SQL Database to Power BI

Open customer_behavior_dashboard.pbix

Create interactive dashboard in Power BI

### Create Project Report and Presentation

Create project report

Build presentation deck using Gamma AI

## Key Insights

Male customers generated higher total revenue than female customers

Loyal customers formed the majority of the customer base

Express shipping users spent more on average

Subscription users showed strong engagement but slightly lower average spend

Certain products had high discount dependency

These findings support strategic marketing and customer retention initiatives. 

