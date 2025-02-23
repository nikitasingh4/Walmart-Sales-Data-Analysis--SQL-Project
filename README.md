# Walmart-Sales-Data-Analysis--SQL-Project
# Walmart Sales Data Analysis - SQL Project

## Overview
This project provides **Sales Insights** using SQL queries on a Walmart sales dataset. The dataset is analyzed to extract meaningful trends, customer behavior, and sales performance metrics. The queries help in business decision-making by answering key sales-related questions.

## Purposes of the Project
The main goal of this project is to gain a deeper understanding of Walmart's sales data by exploring various factors that influence sales across different branches. The project aims to identify high-performing branches and products, analyze sales patterns, and understand customer behavior to enhance and optimize sales strategies.

## About the Data
The dataset used in this project was obtained from the **Kaggle Walmart Sales Forecasting Competition** and includes sales transactions from three Walmart branches located in **Mandalay, Yangon, and Naypyitaw**. The dataset consists of **17 columns and 1000 rows**, providing detailed sales information.

### Dataset Schema
| Column | Description | Data Type |
|--------|------------|-----------|
| invoice_id | Invoice of the sales made | VARCHAR(30) |
| branch | Branch at which sales were made | VARCHAR(5) |
| city | The location of the branch | VARCHAR(30) |
| customer_type | The type of the customer | VARCHAR(30) |
| gender | Gender of the customer making a purchase | VARCHAR(10) |
| product_line | Product line of the product sold | VARCHAR(100) |
| unit_price | The price of each product | DECIMAL(10, 2) |
| quantity | The amount of the product sold | INT |
| VAT | The amount of tax on the purchase | FLOAT(6, 4) |
| total | The total cost of the purchase | DECIMAL(12, 4) |
| date | The date on which the purchase was made | DATETIME |
| time | The time at which the purchase was made | TIME |
| payment | The total amount paid | DECIMAL(10, 2) |
| cogs | Cost Of Goods Sold (COGS) | DECIMAL(10, 2) |
| gross_margin_pct | Gross margin percentage | FLOAT(11, 9) |
| gross_income | Gross Income | DECIMAL(12, 4) |
| rating | Rating | FLOAT(2, 1) |

## Analysis List

### 1. Product Analysis
- Identify top-performing product lines.
- Determine areas for improvement in other product lines.
- Analyze the most common payment methods.
- Evaluate product performance by gender.

### 2. Sales Analysis
- Track sales trends across different time periods.
- Measure revenue by month, branch, and city.
- Identify peak sales hours and high-revenue months.
- Evaluate the effectiveness of sales strategies.

### 3. Customer Analysis
- Identify various customer segments and their purchasing trends.
- Determine the profitability associated with different customer types.
- Analyze customer demographics, including gender distribution.

## Approach Used

### 1. Data Wrangling
- Identify and handle NULL or missing values (though the dataset has NOT NULL constraints).
- Create a structured database and import data.

### 2. Feature Engineering
- **Time_of_day**: Categorizes sales into Morning, Afternoon, and Evening.
- **day_name**: Extracts the day of the week for sales trend analysis.
- **month_name**: Extracts the month of sales for seasonal trend identification.

### 3. Exploratory Data Analysis (EDA)
- Answer business questions and derive insights from sales trends.

## Business Questions to Answer

### Generic Questions
- How many distinct cities are present in the dataset?
- In which city is each branch located?

### Product Analysis
- How many distinct product lines exist in the dataset?
- What is the most common payment method?
- Which product line generates the highest revenue?
- Which city has the highest revenue?
- What is the most common product line by gender?

### Sales Analysis
- How do sales vary by time of day and day of the week?
- Which branch sells more products than the average?
- Which month recorded the highest Cost of Goods Sold (COGS)?

### Customer Analysis
- What is the most common customer type?
- Which customer type generates the highest revenue?
- What is the gender distribution per branch?
- Which time of day has the highest customer ratings?

## How to Use
1. **Set Up the Database:**
   ```sql
   CREATE DATABASE walmart;
   USE walmart;
   ```
2. **Create the Sales Table:**
   Run the table creation SQL query.
3. **Load Data:**
   Modify the `LOAD DATA INFILE` statement with the correct CSV file path and execute it.
4. **Run Analysis Queries:**
   Execute the provided SQL queries to generate sales insights.

## Use Cases
- **Retail Business Decision Making**: Helps store managers and business analysts understand sales performance.
- **Customer Behavior Analysis**: Provides insights into purchasing habits and preferences.
- **Financial Reporting**: Supports revenue tracking, profitability calculations, and financial health assessment.
- **Operational Efficiency**: Helps identify peak hours for staffing and resource allocation.

## Contributing
Feel free to contribute by adding more queries, improving analysis, or optimizing performance.

## License
This project is open-source and available under the [MIT License](LICENSE).

