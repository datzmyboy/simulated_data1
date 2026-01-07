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

* Create a Final_Sales column:

* Cancelled → 0

* Returned → Negative value

* Completed → Net sales

* Create a High_Value_Order flag based on sales thresholds

* Use logical Excel functions such as IF, AND, and OR , ISBLANK

In Task 2, I used Excel functions such as **IF**, **OR**, **ISBLANK**, and **AND** to apply business logic to the dataset. These functions were used to determine which records should be flagged and which data points require further attention. By using logical conditions instead of manual checks, the process ensures consistent validation and helps focus the analysis on records that may impact accuracy and reporting results.







Task 3: Pivot Tables & Management Reporting

Objective: Summarize data for management-level reporting.

 * Build pivot tables for:

 * Total final sales by platform

 * Total quantity sold by product

 * Total returned sales by country

 * Create charts and organize them into a management report sheet


Task 4: Discrepancy & Root Cause Analysis

Objective: Interpret results and identify potential business issues.

* Identify which platform has higher return impact

* ssess whether discounts are associated with return behavior

* Determine which products should be prioritized for audit


The answers for this case study are documented across the Excel worksheets, starting from the raw data and progressing through data validation, analysis, and reporting. Each worksheet reflects a specific task, from the initial raw data review to the final insights provided in Task 4.
 

