# Domino’s Pizza Sales Analysis Using SQL

## 1. Title
**Domino’s Pizza Sales Analysis Using SQL (PostgreSQL)**

---

## 2. Executive Summary
This project demonstrates the use of SQL to explore, clean, and analyze pizza sales and customer data stored in a relational database. Using PostgreSQL, the analysis examines order patterns, revenue distribution, customer behavior, and menu performance. 

By applying joins, aggregations, and window functions across five related tables, the project converts raw transactional data into structured insights that support business decision-making related to pricing, operations, and customer strategy.

---

## 3. Business Problem
Pizza store operations generate large volumes of transactional data across orders, customers, and products. Without structured SQL analysis, it is difficult to answer key business and operational questions such as:

- Which pizzas and categories generate the highest revenue?
- When do customers place the most orders?
- Which customers contribute the most to total sales?
- How is revenue distributed across pizza sizes and categories?

This project was implemented to use SQL as the primary analytical tool to convert relational data into actionable insights that can support pricing decisions, staffing optimization, menu planning, and customer strategy.

---

## 4. Methodology
The analysis is performed using a PostgreSQL relational database consisting of five tables:

- `orders` – order-level information (order date, time, customer)
- `order_details` – item-level details and quantities per order
- `pizzas` – pizza size and pricing data
- `pizza_types` – pizza names and category classifications
- `customers` – customer identification details

### Analytical Workflow
- Verified data integrity and record counts across all tables
- Established relationships using primary and foreign keys
- Performed exploratory analysis using `GROUP BY` and aggregate functions
- Conducted time-based analysis using date and time fields
- Applied window functions for ranking and cumulative trend calculations

All analysis was executed directly using SQL queries.

---

### Analysis & Queries
The following analyses were performed using SQL to evaluate order volume, revenue performance, product trends, time-based demand, and customer behavior.

#### 1. Order Volume Analysis
- Total number of unique orders
- Orders aggregated by month
- Orders aggregated by day of the week
- Average number of orders per customer
- Monthly order trends
- Cumulative order growth trend based on historical data

#### 2. Revenue Analysis
- Total revenue from pizza sales (price × quantity)
- Cumulative revenue trend over time
- Revenue contribution percentage per pizza

#### 3. Product & Menu Performance
- Identification of the highest-priced pizza
- Most frequently ordered pizza size
- Top 5 most ordered pizza types by quantity
- Top 3 pizzas by total revenue
- Top 3 pizzas by revenue within each category

#### 4. Time-Based Analysis
- Orders by hour of the day to identify peak demand periods
- Seasonal trends based on monthly sales patterns

#### 5. Customer Analysis
- Top 10 customers ranked by total spending
- Average order size (number of pizzas per order)
- Customer segmentation into High-Value and Regular customers
- Repeat customer rate compared to one-time buyers

These queries provide a comprehensive view of sales performance, customer purchasing behavior, and operational demand patterns.

---

## 5. Skills & Tools Used

### Technical Skills
- SQL Joins (INNER JOIN, LEFT JOIN)
- Aggregations and Grouping
- Subqueries and Common Table Expressions (CTEs)
- Window Functions
- Time-Series and Trend Analysis
- Business-Oriented Data Analysis

### Tools
- **PostgreSQL** – used for relational data analysis, window functions, and analytical querying
- **pgAdmin** – SQL client used to manage the database and execute queries

---

## 6. Results & Key Insights
- A small set of pizza items contributes a large share of total revenue
- Certain pizza sizes consistently outperform others in revenue generation
- Orders peak during specific hours and weekdays
- High-spending and repeat customers account for a significant portion of sales
- Clear monthly and category-level revenue patterns are observed

---

## 7. Business Recommendations
- Focus promotions on top-performing pizzas and sizes
- Optimize staffing during identified peak ordering hours
- Strengthen retention strategies for high-value customers
- Review pricing or bundling strategies for low-performing menu items
- Use category-level insights to guide menu optimization

---

## 8. Next Steps
- Add revenue forecasting and trend prediction models
- Perform customer lifetime value (CLV) analysis
- Integrate promotional or discount data
- Automate reporting for recurring performance monitoring

---
