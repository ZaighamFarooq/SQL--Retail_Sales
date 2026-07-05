# SQL Retail Sales Analysis

A complete SQL project that walks through the full lifecycle of a retail dataset — from database creation and data cleaning to advanced business intelligence queries. Built as a practical demonstration of core SQL skills for data analysis.

---

## What's Inside

This project works with a retail transaction dataset containing sales records with customer demographics, product categories, timestamps, and financial metrics. The analysis answers ten real-world business questions that any retail analyst would encounter, progressing from basic filtering to advanced window functions and CTEs.

---

## Dataset Overview

| Column | Description |
|--------|-------------|
| `transaction_id` | Unique identifier for each sale (Primary Key) |
| `sale_date` | Date of transaction |
| `sale_time` | Time of transaction |
| `customer_id` | Unique customer identifier |
| `gender` | Customer gender |
| `age` | Customer age |
| `category` | Product category (Clothing, Beauty, Electronics, etc.) |
| `quantity` | Units purchased |
| `price_per_unit` | Retail price per item |
| `cogs` | Cost of Goods Sold |
| `total_sale` | Final transaction amount |

---

## Business Questions Answered

1. **Daily Sales Snapshot** — Retrieve all transactions for a specific date (`2022-11-05`)
2. **Category & Volume Filtering** — Clothing sales in November 2022 with quantity ≥ 4
3. **Category Performance** — Total sales and order count by product category
4. **Customer Demographics** — Average age of customers purchasing Beauty products
5. **High-Value Transactions** — All sales exceeding $1,000
6. **Gender-Category Matrix** — Transaction count broken down by gender and category
7. **Best Month Per Year** — Monthly average sales ranked within each year to identify peak performance
8. **Top Customers** — Top 5 customers by total lifetime spend
9. **Category Reach** — Unique customer count per category (market penetration)
10. **Shift Analysis** — Order volume by time-of-day shift (Morning/Afternoon/Evening)

---

## SQL Techniques Demonstrated

- **Data Cleaning**: Null value detection and deletion across critical fields
- **Aggregation**: `COUNT`, `SUM`, `AVG`, `ROUND` with `GROUP BY`
- **Filtering**: `WHERE` clauses with multiple conditions and date formatting
- **Window Functions**: `RANK() OVER (PARTITION BY ...)` for intra-group ranking
- **CTEs**: `WITH` clauses for modular, readable shift categorization
- **Date/Time Extraction**: `EXTRACT()` for year, month, and hour parsing
- **Deduplication**: `COUNT(DISTINCT)` for unique customer metrics

---


---

## How to Run

1. Create a new database:
   ```sql
   CREATE DATABASE sql_p;
2. Execute the table creation and data insertion scripts.
3. Run queries sequentially — the project is organized into logical sections:
   Database & Table Setup
   Data Cleaning
   Exploratory Analysis
   Business Intelligence Queries

Key Insights
   Data Quality First: The project begins with comprehensive null-checking across all critical columns before any analysis, ensuring           reliable downstream metrics.
   Time Intelligence: Shift analysis and monthly ranking demonstrate how to extract actionable business intelligence from raw timestamps.
   Granular Segmentation: The gender-category matrix and unique customer counts show how to slice data for targeted marketing insights.
   
Tools Used
   SQL (PostgreSQL-compatible syntax)
   Standard SQL functions and window operations.
    
Connect
If you're working through similar SQL projects or have suggestions for additional analyses, feel free to reach out or open an issue.
