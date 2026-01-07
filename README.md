# Simulated Excel Data Analyst Case Study


After applying for entry-level data analyst roles, I realized that most companies in my area prioritize strong Excel skills for junior positions, even before Python or SQL. To address this gap, I decided to create a simulated case study based on real job descriptions for entry-level data analyst roles. I used these job requirements as a reference and prompted AI to act as a manager, assigning realistic tasks while I assumed the role of the data analyst. This project demonstrates how I approach data validation, Excel-based analysis, reporting, and business insights in a practical, job-relevant context.

Below are the task requirements generated based on entry-level data analyst job descriptions, which I followed to complete this case study.


# Task 1: Data Validation & Internal Control

  Objective: Ensure the dataset is reliable and ready for analysis.

  * Check for missing values

  * Identify negative prices or quantities

  * Flag orders marked as Cancelled or Returned that still contribute to sales

  * Create a Data_Issue_Flag column to mark problematic records
    
In Task 1, I created a helper column called **Date_issue_flag**. This column is used to identify whether certain data values may be inaccurate or require review. It checks for blank values, as missing data can affect total calculations and reporting accuracy. It also checks if net sales values are negative, which helps identify parts of the data that need further attention. In addition, the order status is reviewed to determine whether an order is marked as Returned or Cancelled, since these statuses directly affect profit and should not be treated the same as completed sales. If any of these conditions are met, the row is flagged as “YES”; otherwise, it is marked as “NO”.











# Task 2: Excel Formula Proficiency

Objective: Apply business logic using Excel formulas.

* Create a **Final_sales column**:

* Create a **High_value_order** flag based on sales thresholds

* Use logical Excel functions such as IF, AND, and OR , ISBLANK

In Task 2, I used Excel functions such as **IF**, **OR**, **ISBLANK**, and **AND** to apply business logic to address the inaccurate data identified in Task 1, specifically through the Date_Issue_Flag. These functions were used to determine which data values required further attention. In addition, a **Final_sales** column was created to represent the actual financial impact of each order based on its status, assigning negative values for returned orders and zero values for cancelled orders. I also created a **High_value_order** column using gross sales to identify transactions that require closer monitoring, as these high-value products can significantly affect overall sales performance if not handled properly.


![Project Screenshot](https://github.com/datzmyboy/simulated_data1/blob/main/data1_pic.jpg)




# Task 3: Pivot Tables & Management Reporting

Objective: Summarize data for management-level reporting.

 * Build pivot tables for:

 * Total final sales by platform

 * Total quantity sold by product

 * Total returned sales by country

 * Create charts and organize them into a management report sheet

In Task 3, I created pivot tables to summarize total final sales by platform, total quantity sold by product, and the sum of returned final sales by country. Through these tables, I was able to identify sales and return trends and use them to support future business analysis and decision-making.

The pivot tables can be found in the Task 3 worksheet of the workbook or in the Management_Report sheet. The file contains multiple tables across different tasks, including those used in Task 4, so a single screenshot does not capture all of them.






# Task 4: Discrepancy & Root Cause Analysis

Objective: Interpret results and identify potential business issues.

* Identify which platform has higher return impact

* ssess whether discounts are associated with return behavior

* Determine which products should be prioritized for audit
![Project Screenshot](https://github.com/datzmyboy/simulated_data1/blob/main/Screenshot%202026-01-08%20072627.png)



