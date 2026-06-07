Project Overview
This project analyzes retail sales performance using SQL in Databricks. The goal is to uncover business insights related to sales, profitability, product performance, customer segments, shipping methods, and regional trends.
The analysis demonstrates practical business intelligence skills, including data exploration, KPI development, profitability analysis, and data visualization.

Business Objectives
Identify the most profitable product categories
Evaluate sales performance across regions
Understand the impact of discounts on profitability
Compare customer segments and shipping methods
Provide actionable recommendations to improve business performance

Tools & Technologies
Databricks
Spark SQL
GitHub
Databricks Visualizations

Project Workflow
Data Import
    ↓
Data Validation
    ↓
Data Cleaning
    ↓
Exploratory Analysis
    ↓
Business Insights
    ↓
Visualizations
    ↓
Recommendations

SQL Analysis

Total Sales and Profit
SELECT
    SUM(Sales) AS total_sales,
    SUM(Profit) AS total_profit
FROM sales_superstore;

Sales by Category
SELECT
    Category,
    SUM(Sales) AS revenue
FROM sales_superstore
GROUP BY Category
ORDER BY revenue DESC;

Profit by Region
SELECT
    Region,
    SUM(Profit) AS profit
FROM sales_superstore
GROUP BY Region
ORDER BY profit DESC;

Visualizations
The project includes:
Sales by Category
Profit by Region
Sales by Customer Segment
Sales by Shipping Mode
Discount vs Profit Analysis
Top Performing Product Categories

Key Insights
Examples of insights that can be derived from this analysis:
Certain product categories contribute significantly more revenue than others.
Some regions generate high sales but relatively low profit.
Higher discount levels may negatively impact profitability.
Customer segments show different purchasing behaviors.
Shipping preferences vary across customer groups.

Business Recommendations
Based on the findings:
Focus marketing efforts on high-profit categories.
Review discount strategies to protect margins.
Investigate underperforming regions.
Optimize shipping methods to improve customer experience.
Develop targeted strategies for different customer segments.

Repository Structure
retail-sales-analytics/
│
├── README.md
├── data/
├── sql/
│   ├── data_validation.sql
│   ├── exploratory_analysis.sql
│   └── business_insights.sql
│
├── visualizations/
│   ├── sales_by_category.png
│   ├── profit_by_region.png
│   └── discount_analysis.png
│
└── docs/
    └── insights_summary.md
    
Skills Demonstrated
SQL Query Development
Data Exploration
Business Intelligence
KPI Reporting
Data Visualization
Analytical Thinking
Data Storytelling
