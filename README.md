# Project_3_SQL_analysis
# Order Records - SQL Data Analysis

## Overview
This project is the third phase of a data analytics internship at DecodeLabs. Building on the cleaned dataset from Project 1 and the exploratory analysis from Project 2, this notebook moves from pandas based exploration into structured SQL querying, using SQLite to answer specific business questions about revenue, operations, and customer acquisition.

## Dataset
* 1,200 order records spanning January 2023 to June 2025
* 14 columns covering products, pricing, payment methods, order status, and referral sources
* Loaded into a SQLite database (`orders.db`) for direct SQL querying

## What's Inside the Notebook
* Revenue analysis by product, payment method, and average order value
* Monthly revenue trends using date extraction (`strftime`)
* Cancellation analysis by product and by payment method, using rate calculations rather than raw counts
* Coupon usage comparison between cancelled orders and the dataset as a whole
* Referral source analysis comparing raw order volume against delivery conversion rate
* All 8 questions answered using SELECT, WHERE, GROUP BY, ORDER BY, and aggregate functions (COUNT, SUM, AVG)

## Key Findings
* Chair leads in total revenue, driven by higher average quantity per order rather than price or order count
* Revenue is fairly evenly distributed across payment methods, no single method dominates
* June shows a recurring pattern of strong revenue across all three years in the dataset
* Cancellation rates vary only modestly by product and payment method, no clear outlier
* Coupon usage among cancelled orders closely mirrors coupon usage across all orders, ruling it out as a driver of cancellations
* Instagram drives the most referral traffic, but Email converts at a notably higher delivery rate (24.00% vs 20.08%)
* Referral is the weakest acquisition channel on both volume and delivery rate

## Tools Used
* Python 3
* pandas
* sqlite3
* Jupyter Notebook

## Author
Daniel | DecodeLabs Data Analytics Internship, Batch 2026
