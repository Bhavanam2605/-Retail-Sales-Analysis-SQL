# -Retail-Sales-Analysis-SQL

#Overview
This project presents a structured analysis of retail sales data using SQL. It demonstrates core data analytics skills including data cleaning, exploratory data analysis, and business insight generation. The objective is to analyze transactional data to identify sales trends, customer behavior, and category performance.

#Dataset Description
The dataset consists of transactional retail sales records. Each record represents a single purchase and contains information related to the customer, product category, and transaction details.

| Column Name    | Description                    |
| -------------- | ------------------------------ |
| transaction_id | Unique transaction identifier  |
| sale_date      | Date of transaction            |
| sale_time      | Time of transaction            |
| customer_id    | Unique customer identifier     |
| gender         | Customer gender                |
| age            | Customer age                   |
| category       | Product category               |
| quantity       | Number of units sold           |
| price_per_unit | Price per unit                 |
| cogs           | Cost of goods sold             |
| total_sale     | Total value of the transaction |

#Data Preparation
Data cleaning was performed to ensure accuracy and consistency. Records with missing or null values in key fields were removed. This step ensures that the analysis is based on reliable and complete data.

#Key Analysis
The project focuses on solving business-relevant analytical problems using SQL. The analysis includes:
Evaluation of sales trends over time
Identification of top-performing product categories
Customer segmentation based on demographics
Detection of high-value transactions
Ranking of customers based on total spending
Analysis of sales distribution across different times of the day

#Sample Query
Below is an example query used to identify the top customers based on total spending:

SELECT customer_id, SUM(total_sale) AS total_spent
FROM retail_sales
GROUP BY customer_id
ORDER BY total_spent DESC
LIMIT 5;

#Key Insights
Sales tend to increase during specific periods, indicating seasonal trends
Certain product categories consistently generate higher revenue
A small group of customers contributes significantly to overall sales
Customer purchasing behavior varies across different times of the day

#Tools and Technologies
SQL

#Project Files
retail_sales.sql contains all SQL queries used in the analysis
README.md provides project documentation
dataset.csv contains the raw dataset if included

#Conclusion
This project demonstrates the practical application of SQL in analyzing real-world business data. It highlights the ability to transform raw data into meaningful insights that can support decision-making.
