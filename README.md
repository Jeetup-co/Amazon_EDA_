🛒 Amazon Products & Reviews – End-to-End Data Analysis Project
📌 Project Overview

This project is a complete end-to-end data analysis pipeline built using Python and SQL (SQLite).
The goal of the project is to analyze Amazon product listings and customer reviews to uncover insights related to customer engagement, pricing strategies, discounts, and product quality.

The project simulates a real-world data analyst workflow:

Data Cleaning → Exploratory Data Analysis → SQL Analytics

🎯 Business Objectives

Identify top-performing categories and products

Analyze customer engagement using review counts

Understand the impact of pricing and discount strategies

Detect bad-quality products (high discount + low rating)

Build analysis-ready datasets using SQL

🗂️ Dataset Description

The dataset contains Amazon product and review information with the following columns:

product_id, product_name, category,
discounted_price, actual_price, discount_percentage,
rating, rating_count,
about_product,
user_id, user_name,
review_id, review_title, review_content,
img_link, product_link

🛠️ Tools & Technologies Used
🐍 Python

pandas

numpy

matplotlib / seaborn

Data cleaning & feature engineering

Exploratory Data Analysis (EDA)

🗄️ SQL (SQLite)

Database design & normalization

JOIN, GROUP BY, HAVING

Analytical SQL queries

🔄 Project Workflow
1️⃣ Python – Data Cleaning & EDA

Removed special characters from price columns

Converted prices and discounts to numeric format

Cleaned category hierarchy

Handled missing values

Created new features (price ranges, rating buckets)

Performed exploratory analysis:

Category performance

Price vs rating analysis

Discount impact

Identification of risky products

2️⃣ SQL (SQLite) – Data Modeling & Analysis

Designed normalized database schema:

products table

reviews table

Inserted cleaned data into SQLite

Performed SQL analytics:

Total products & reviews

Top categories by engagement

Best-rated categories

Most reviewed products

Highest discount products

Bad-quality products (high discount + low rating)

📊 Key Insights

Electronics is the most dominant category with the highest customer engagement.

Mid-range products receive the highest review volumes.

Premium products receive fewer reviews but higher average ratings.

Several products rely on heavy discounts (70%+) despite low ratings, indicating quality concerns.

Brands like AmazonBasics, boAt, and Redmi dominate high-volume product segments.

📁 Repository Structure
├── data/
│   ├── amazon_cleaned.csv
│
├── sql/
│   ├── amazon.db
│
├── exports/
│   ├── category_performance.csv
│   ├── top_products.csv
│   ├── highest_discount_products.csv
│   ├── bad_quality_products.csv
│
├── notebooks/
│   ├── amazon_eda.ipynb
│
└── README.md

🚀 How to Run This Project

Clone the repository

Open the Jupyter Notebook for Python EDA

Run SQL analysis using SQLite

Review insights generated from SQL queries

💡 Future Improvements

Add sentiment analysis on review text

Use PostgreSQL/MySQL for scalability

Automate data pipeline

Integrate advanced analytics

👤 Author

Jitendra Kumar
Aspiring Data Analyst | Python | SQL
