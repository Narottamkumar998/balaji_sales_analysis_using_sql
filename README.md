🍔 Balaji Fast Food Sales Analysis

A MySQL database project that analyzes Balaji Fast Food sales transactions to identify sales trends, product performance, customer payment preferences, and potential revenue opportunities.

📌 Project Overview

This project uses SQL queries to explore sales data for Balaji Fast Food. It focuses on total revenue and orders, product-level performance, category-wise revenue, payment methods, average order value, and sales patterns across different times of day.

The analysis is intended to turn transaction records into practical business insights and recommendations.

🎯 Objectives

Calculate total revenue and total orders.

Identify the best-selling products by quantity.

Find the products generating the highest revenue.

Compare revenue from Fast Food and Beverages.

Compare Cash and Online payment methods by revenue and order count.

Calculate average order value and effective revenue per unit sold.

Examine sales patterns by time of day.

Recommend actions that may help improve sales and operations.

🛠️ Tools & Technologies

MySQL — database creation, data querying, aggregation, and analysis

SQL — SUM(), COUNT(), AVG(), MAX(), GROUP BY, ORDER BY, and LIMIT

🗂️ Database Structure

Database: sales_analysis
Table: sales

The sales table contains 10 columns:

Column

Purpose

order_id

Order identifier

date

Transaction date

item_name

Product name

item_type

Product category

item_price

Item price

quantity

Quantity sold

transaction_amount

Transaction amount

transaction_type

Payment method, such as Cash or Online

received_by

Staff member who received the order

time_of_sale

Time-of-day category

📊 Key Results

The following figures are reported in the project's sales analysis presentation and summary report.

Metric

Result

Total revenue

₹53,626

Total orders / transaction rows

2,000

Average order value

₹26.81

Top-selling item by quantity

Sandwich — 312 units

Highest-revenue product

Cold Coffee — ₹12,450

Second-highest-revenue product

Sandwich — ₹9,870

Third-highest-revenue product

Shake — ₹8,340

Fast Food revenue

₹31,200 (58.2%)

Beverage revenue

₹22,426 (41.8%)

Cash revenue

₹28,410 (about 53%)

Online revenue

₹25,216 (about 47%)

Cash transactions

1,063 (53.2%)

Online transactions

937 (46.8%)

Highest listed item price

Shake — ₹80

Highest effective revenue per unit among highlighted products

Shake — ₹52.10 per unit

Note: “Revenue per unit” is the effective amount per unit sold, calculated as total transaction amount divided by total quantity. It should not automatically be interpreted as profit or profit margin because product costs are not included in the reported analysis.

🔎 SQL Analysis Performed

The project demonstrates queries and analysis for:

Database setup — creating and selecting the sales_analysis database.

Table creation and inspection — defining the sales table and using DESCRIBE sales.

Total revenue — calculating SUM(transaction_amount).

Order count — counting rows in the sales table.

Top-selling products — summing quantity by item_name.

Revenue by product — summing transaction amounts by product.

Category revenue — comparing Fast Food and Beverage sales.

Payment analysis — comparing Cash and Online revenue and transaction counts.

Average order value — calculating AVG(transaction_amount).

Top three products by revenue — sorting products and using LIMIT 3.

Time-of-day analysis — examining revenue by date and sales time.

Highest item prices — using MAX(item_price) for each product.

Revenue per unit — dividing total transaction amount by total quantity for each product.

💡 Business Insights

Sandwich leads by quantity: 312 units were sold, making it the top-selling item by units.

Cold Coffee leads by revenue: It generated ₹12,450 in reported revenue.

Fast Food contributes more revenue: Fast Food accounted for ₹31,200 (58.2%) compared with ₹22,426 (41.8%) from Beverages.

Payment preferences are relatively balanced: Cash contributed about 53% of revenue and Online payments about 47%.

Evening is identified as the peak sales period in the project presentation.

Shake has the highest listed item price: ₹80. The analysis also reports ₹52.10 effective revenue per unit for Shake; this is not a profit calculation.
