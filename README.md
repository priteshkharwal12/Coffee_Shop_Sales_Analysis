# Coffee Shop Sales: End-to-End Data Analysis Project

This repository contains an end-to-end data analysis project focused on coffee shop sales. The project involves using **MySQL** for data cleaning and querying, and **Power BI** for creating a dynamic and interactive dashboard. This project is designed to showcase the practical application of data analysis skills, from raw data preparation to insightful visualisation.

## Project Overview

The core objective of this project is to analyse sales data for a coffee shop to provide key insights and answer specific business questions. This involves a two-part process:

1.  **MySQL Data Analysis**: The first part focuses on using MySQL to prepare and analyse the raw data. This includes data cleaning, data type conversion, and running complex SQL queries to validate metrics and extract preliminary insights based on business requirements.
2.  **Power BI Dashboard Creation**: The second part involves building a comprehensive, interactive, and dynamic dashboard in Power BI. This dashboard visualises key performance indicators (KPIs) and provides granular insights through various charts and heat maps.

The raw data for this project can be downloaded from the link provided in the video description. The dataset contains approximately 150,000 rows of transactional sales data for the first six months of 2023.

## Key Features of the Power BI Dashboard

The final dashboard is a high-level, dynamic tool designed to provide a comprehensive overview of the coffee shop's performance.

### **KPIs and Headers**
*   **Total Sales**: Overall revenue generated.
*   **Total Orders**: Total number of transactions.
*   **Total Quantity Sold**: Total number of items sold.
*   Each KPI is accompanied by a **month-on-month (MoM) growth/decline percentage** and a sparkline showing the daily trend.

### **Interactive Visualisations & Charts**
*   **Calendar Heat Map**: Dynamically adjusts to the selected month, with days colour-coded based on sales volume. Tooltips display daily sales, orders, and quantity.
*   **Sales vs. Weekday/Weekend**: A customised chart analysing sales patterns on weekdays versus weekends.
*   **Sales by Store Location**: A customised stacked bar chart comparing the performance of different store locations, including MoM metrics.
*   **Daily Sales Trend with Average Line**: A column chart showing daily sales against the monthly average, highlighting days with above-average performance.
*   **Sales by Product Category**: Analysis of sales performance across different product categories.
*   **Top 10 Products by Sales**: Identifies the best-performing products to inform marketing and inventory decisions.
*   **Sales by Day and Hour Heat Map**: A heat map visualising sales patterns at different hours on different days of the week, with detailed tooltips.

### **Dynamic Functionality**
*   **Month Slicer**: Allows users to filter the entire dashboard for a specific month, with all visualisations updating dynamically.
*   **Interactive Filters**: Users can click on elements within charts (e.g., 'weekends' in the sales chart, a specific store location, or a product category) to filter the entire dashboard and deep-dive into the data.

## Project Workflow & Technical Skills

This project follows a structured workflow, starting from data preparation in MySQL to final visualisation in Power BI.

### **Part 1: MySQL Database Operations**

1.  **Data Preparation**: The initial Excel file (`.xlsx`) is converted to a CSV (`.csv`) format suitable for import into MySQL.
2.  **Database & Table Creation**: A new database and table are created to house the sales data.
3.  **Data Import**: The CSV file is imported into the MySQL table using the Table Data Import Wizard.
4.  **Data Cleaning**: SQL queries are used for essential data cleaning tasks:
    *   **Changing Data Types**: The `transaction_date` and `transaction_time` columns are converted from `TEXT` to `DATE` and `TIME` data types, respectively, using `STR_TO_DATE` and `ALTER TABLE...MODIFY COLUMN` statements.
    *   **Renaming Columns**: The `transaction_id` column name is corrected to remove extraneous characters imported by the wizard using `ALTER TABLE...CHANGE COLUMN`.
5.  **SQL for Business Requirements**: Advanced SQL queries are written to calculate and validate the metrics needed for the dashboard. This is a crucial step for cross-checking the accuracy of the dashboard's figures. Key calculations include:
    *   Total Sales, Orders, and Quantity for a selected month.
    *   Month-on-Month (MoM) growth using window functions like `LAG()`.
    *   Sales by day, weekday/weekend, store location, and product category using `CASE` statements and `GROUP BY` clauses.
    *   Calculating average daily sales using subqueries.

### **Part 2: Power BI Dashboard (To be completed)**
The second part of the project will focus on connecting to the MySQL database (or the cleaned data) and building the dashboard as described above, utilising DAX for calculations and Power Query for any additional transformations.

## Skills Demonstrated
*   **Database Management (MySQL)**: Data import, cleaning, schema creation, and writing advanced SQL queries (Joins, Aggregations, Window Functions, Subqueries, CTEs).
*   **Data Visualisation (Power BI)**: Creating interactive and dynamic dashboards, DAX calculations, implementing filters and slicers, and using custom visuals.
*   **Business Intelligence**: Translating business requirements into KPIs and data visualisations, deriving actionable insights from data.
*   **ETL Processes**: Basic extraction, transformation (cleaning), and loading of data into a database.

***
