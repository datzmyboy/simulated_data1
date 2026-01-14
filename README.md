# Simulated Excel Data Analyst Case Study
After applying for entry-level data analyst roles, I realized that most companies in my area prioritize strong Excel skills for junior positions, often even before Python or SQL. To address this gap, I created a simulated Excel data analyst case study based on real job descriptions for entry-level roles.

I used these job requirements as a reference and prompted AI to act as a manager by generating realistic task requirements, similar to how assignments are given in a real work environment. I then independently completed all data validation, Excel-based analysis, reporting, and interpretation using the provided dataset.

This project demonstrates my approach to data quality checks, business logic implementation using Excel formulas, pivot table analysis, and translating data findings into meaningful business insights. The tasks listed below simulate real-world analyst responsibilities, while all calculations, analysis, and conclusions reflect my own work and understanding of the data.



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
This screenshot is from the main Excel file, specifically the Task_4 worksheet. I included a screenshot because it contains the same answers shown in the analysis.

# Final Insights & Recommendations

In this case study, we found that Shopify generated higher final sales compared to Amazon. The analysis also showed that having more discounts or higher discount levels does not strongly correlate with higher returns, suggesting that other factors need to be monitored. Since returned sales are sometimes inevitable and part of normal business operations, the company should focus on monitoring and strengthening areas that generate higher profit to help offset potential losses. Products that are sold in high quantities and generate significant sales should be prioritized for audit to maintain or improve performance and to reduce the risk of future returns and negative customer feedback.


# Bonus
Although not part of the main task requirements, this bonus section was added to demonstrate practical use of the VLOOKUP function, which is a commonly expected skill for entry-level data analyst roles. A small sample dataset was generated for this purpose, and VLOOKUP was used to retrieve missing reference information and enrich the data.


