# 📊 Data Engineering Project – Data Warehouse in Databricks

##📌 Overview

This project demonstrates the design and implementation of a small Data Warehouse (DW) using Databricks, Apache Spark, and SQL.
The solution follows the Medallion Architecture (Bronze, Silver, Gold layers) and implements an ETL process to transform raw CSV data into structured analytical datasets.
The goal of this project is to showcase core data engineering concepts such as data ingestion, transformation, and modeling using a dimensional approach.

## 🏗️ Architecture

The project is built using the Medallion Architecture, which consists of three layers:

Bronze Layer (Raw Data)
Stores raw CSV files as-is
Data is ingested without transformation
Silver Layer (Cleaned Data)
Data cleaning and standardization
Handling nulls, data types, and inconsistencies
Gold Layer (Business-Level Data)
Data modeled into a star schema
Optimized for analytics and reporting

## 🔄 ETL Process

The ETL pipeline includes the following steps:

Extract
Load CSV files into Databricks using Spark
Transform
Clean and validate data
Apply business rules
Normalize and structure datasets
Load
Store processed data into Delta tables
Organize into dimensional model (Gold layer)

## 🧱 Data Model

The final Data Warehouse follows a Star Schema with:

### 🔹 Dimension Tables
brands
category
products
customers
(Note: If you actually have 5 dimensions, include the missing one here if applicable)
### 🔸 Fact Table
order_items

The fact table stores transactional data and connects to all dimension tables through surrogate or business keys.

## 📂 Data Sources
All data used in this project comes from CSV files, which simulate raw input from external systems.

## ⚙️ Technologies Used
Databricks
Apache Spark (PySpark)
SQL
Delta Lake
CSV (Raw Data Source)

## 📊 Key Features
Implementation of Medallion Architecture
End-to-end ETL pipeline
Use of Spark for scalable data processing
Dimensional modeling using a Star Schema
Data stored in Delta format for performance and reliability

## 🚀 How to Run the Project
Upload CSV files into Databricks (DBFS or workspace)
Execute notebooks in the following order:
Bronze ingestion
Silver transformation
Gold modeling
Validate tables using SQL queries

## 📈 Future Improvements
Add data quality checks (e.g., Great Expectations)
Automate pipelines using workflows
Integrate visualization tools (Power BI / Tableau)
Expand dataset and include more fact tables

## 🌟 About Me

Hi there! I'm **Adrián Fajardo**. I’m a Future Systems Engineer who is looking to create, share and contribuite with amazing projects. The areas I want to specialize are data engineering and data analytics. Join me and let's learn together.

Let's stay in touch! Feel free to connect with me on the following platforms:

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](www.linkedin.com/in/adrián-yusef-fajardo-huamaní-a38170270)
