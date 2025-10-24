🧠 Data Analysis Projects using SQL

📘 Overview

This repository contains two SQL-based data analysis projects:

1. A Mini Project focusing on business insights from an e-commerce dataset.


2. An EDA Project (Exploratory Data Analysis) performed completely in SQL, aimed at discovering hidden patterns and relationships in the data.



Both projects demonstrate my ability to use SQL for data exploration, analysis, and insight generation.


---

🧩 Project 1 — SQL Mini Project: E-Commerce Business Insights

🎯 Objective

To analyze e-commerce product data using SQL and extract insights about pricing, discounts, and stock management.

🗂 Dataset Details

Column	Description

category	Product category
productName	Name of the product
price	Original price
discountedSellingPrice	Discounted price
quantity	Quantity available
stock	Stock availability
weight	Product weight in grams


⚙ Key SQL Analyses

Average and discounted price comparison by category

Identifying categories with high discounts

Product classification based on price ranges

Stock and quantity analysis


🧠 Example Query

SELECT 
    category,
    ROUND(AVG(discountedSellingPrice), 2) AS avg_discounted_price,
    ROUND(AVG(price), 2) AS avg_price,
    ROUND(AVG(discountedSellingPrice) / AVG(price) * 100, 2) AS discount_percent
FROM categories
GROUP BY category
ORDER BY discount_percent ASC;

💡 Insights

Categories with >30% discount tend to sell faster.

Medium-priced products (₹500–₹2000) dominate sales.

Understocked categories indicate areas for restocking and inventory improvement.



---

🧮 Project 2 — SQL EDA Project: Exploratory Data Analysis using SQL

🎯 Objective

To perform Exploratory Data Analysis (EDA) directly through SQL queries — identifying trends, outliers, and statistical summaries without external tools.

🔍 EDA Steps Implemented in SQL

1. Data Cleaning: Handling missing or inconsistent values.


2. Descriptive Statistics: Using AVG(), MAX(), MIN(), and COUNT() to understand dataset structure.


3. Categorical Analysis: Grouping data by categories and ranges.


4. Outlier & Trend Detection: Using conditions and subqueries.



🧠 Example Query

SELECT 
    category,
    COUNT(*) AS total_products,
    ROUND(AVG(price), 2) AS avg_price,
    ROUND(STD(price), 2) AS price_std_dev
FROM categories
GROUP BY category
ORDER BY avg_price DESC;

💡 Key Findings

High-priced categories have greater price variability.

Some categories consistently maintain stable pricing, showing low volatility.

SQL-based EDA provided fast and interpretable data summaries without Python or BI tools.



---

🧠 Skills Demonstrated

Advanced SQL Querying

Data Cleaning and Transformation

Statistical & Business Analysis

EDA using SQL Functions

Problem Solving with Real-World Data



---

🛠 Tools Used

Language: SQL

Environment: MySQL 

Dataset: E-Commerce Product Dataset

Category: Data Analytics & Business Intelligence



---

👤 Author

Pathan Afridh Khan
📅 October 2025
📂 SQL Mini Project & SQL EDA Project
