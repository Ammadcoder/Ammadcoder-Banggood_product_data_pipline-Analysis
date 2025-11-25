Banggood Product Data Pipeline & Analysis

An end-to-end data engineering and analytics project that scrapes product data from Banggood.com, cleans and analyzes it using Python, and stores the final dataset in SQL Server for further insights.

🚀 Project Overview

This project demonstrates a complete workflow:

Web Scraping

Data Cleaning & Transformation

Exploratory Data Analysis (Python)

SQL Server Loading

SQL Aggregated Analysis

Final Reporting

📦 Features
🔍 Part 1: Web Scraping

Scrapes 5 Banggood categories

Extracts:

Product name

Price

Rating

Review count

Product URL

Uses:

requests

BeautifulSoup

Selenium (for dynamic content)

Pagination support for multi-page scraping

🧹 Part 2: Data Cleaning & Transformation

Performed using pandas

Cleaning operations include:

Converting price → float

Parsing ratings

Fixing review count format

Handling missing values

Added derived features:

value_score = (rating * reviews) / price

discounted_price (if discount info exists)

📊 Part 3: Exploratory Data Analysis (Python)

Includes minimum 5 insights such as:

Price distribution per category

Rating vs price correlation

Top reviewed products

Best value items

Stock/availability trends

Visualizations using Matplotlib

💾 Part 4: SQL Server Loading

Designed database schema

Loaded cleaned data using:

pyodbc

Validated rows using SQL queries

Supports:

Separate tables per category

Or single unified table

📈 Part 5: SQL Aggregated Analysis

Includes SQL queries such as:

Average price per category

Average rating per category

Total products

Top 5 reviewed products

Stock availability percentage

📘 Part 6: Final Report

The report includes:

System architecture diagram

Data scraping explanation

Cleaning & transformation workflow

Python analysis with graphs

SQL insights & final recommendations

🛠️ Tech Stack

Python: Requests, BeautifulSoup, Selenium, Pandas

Database: SQL Server

Visualization: Matplotlib

Connector: pyodbc
          
          📂 Project Structure
          📁 Banggood-Product-Pipeline
          │
          ├── scraping/
          │   └── banggood_scraper.py
          ├── cleaning/
          │   └── data_cleaning.py
          ├── analysis/
          │   ├── python_eda.ipynb
          │   └── sql_queries.sql
          ├── database/
          │   └── schema.sql
          ├── report/
          │   └── Final_Report.pdf
          └── README.md
            
✔️ How to Run

Install requirements

Run scraper

Clean and transform data

Perform EDA

Load into SQL Server

Run SQL analyses
