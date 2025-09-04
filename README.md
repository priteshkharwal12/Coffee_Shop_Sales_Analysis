Of course. Here is a project summary for your Coffee Shop Sales Analysis, following the format you provided.

***

### Coffee Shop Sales Analysis Project:
☕☕☕☕☕

**Objective:** To analyse coffee shop sales data to identify key performance indicators (KPIs), understand sales patterns, and provide actionable insights for business growth.

**About the Dataset:**
The dataset contains detailed transactional sales information for a coffee shop, covering the first six months of 2023. It includes approximately 150,000 rows and 11 columns, with details such as transaction ID, date, time, quantity sold, store location, unit price, and product category. This data is crucial for understanding sales performance and operational patterns.

**Business Problem:**
Analyse the coffee shop's sales data to identify trends and provide insights to answer specific business questions. The goal is to create a dynamic, high-level dashboard that allows the client to deep-dive into the data at a granular level, helping them understand business performance and make informed decisions.

**Tools Used:**
*   **MySQL:** For data import, cleaning, preparation, and firing advanced SQL queries to validate business metrics.
*   **Power BI:** For creating a dynamic, interactive, and customised dashboard for visualisation and analysis.

**Project Workflow:**

*   **Data Cleaning (MySQL):** The raw Excel (`.xlsx`) file was converted to CSV (`.csv`) and imported into a MySQL database. SQL queries were used to clean the imported data, including:
    *   Correcting the `transaction_id` column name using `ALTER TABLE...CHANGE COLUMN`.
    *   Converting `transaction_date` and `transaction_time` from `TEXT` to `DATE` and `TIME` data types using `STR_TO_DATE`, `UPDATE`, and `ALTER TABLE...MODIFY COLUMN` statements.

*   **Data Analysis (SQL & Power BI):**
    *   **KPIs:** Calculated total sales, total orders, and total quantity sold. This included month-on-month (MoM) growth and the difference between the selected month and the previous month.
    *   **Sales Trends:** Evaluated daily sales trends against a monthly average to identify high-performing and low-performing days.
    *   **Top Products:** Identified the top 10 best-selling products to inform marketing and inventory strategies.
    *   **Pattern Analysis:** Analysed sales performance based on day of the week (weekday vs. weekend) and by the hour to identify peak sales times.
    *   **Location Analysis:** Assessed and compared sales performance across the three different store locations.

*   **Visualisation (Power BI):** Created a comprehensive and interactive dashboard using custom charts and advanced DAX calculations. Key visuals include:
    *   A dynamic **calendar heat map** that adjusts based on the selected month, with tooltips showing daily metrics.
    *   A **daily and hourly heat map** to visualise sales patterns.
    *   Customised bar charts for store locations and product categories, showing MoM growth directly on the visual.
    *   A column chart for **daily sales with an average line**, highlighting days performing above or below the monthly average.

**Business Recommendations:**
The analysis provides a basis for strategic actions. For instance:
*   Focus marketing efforts on the **top-selling products** (e.g., Barista Espresso) to maximise revenue.
*   Optimise staffing and inventory during **peak hours (7 AM - 10 AM)**, which consistently show the highest sales volume.
*   Develop targeted promotions for weekdays, as days like Monday, Tuesday, and Wednesday show the highest sales, potentially due to office rushes.

**Result:** Provided a comprehensive, dynamic dashboard and validated SQL queries that deliver clear insights into sales performance. This enables the business to enhance sales, improve customer satisfaction by understanding preferences, and streamline operations based on identified trends. operations based on identified trends.
