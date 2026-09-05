
# Supply Chain Analytics Dashboard

An end-to-end data analytics project that looks at how a distribution business manages its supply chain — from the moment an order is placed to the moment it's delivered. The project covers data cleaning, SQL analysis, and an interactive Power BI dashboard.

# Introduction

Any business that moves physical goods — from a supplier, through a warehouse, to a customer — relies on a supply chain made up of many moving parts: orders, suppliers, warehouses, and customers spread across different sales channels. This project uses a real-world style operational dataset covering order transactions, inventory movements, supplier details, and customer information to understand how well a supply chain is actually performing.

# Problem Statement

Businesses often struggle to get a clear, connected view of how day-to-day operational issues affect overall performance. Deliveries are sometimes late, certain warehouses run out of stock more often than others, some suppliers are less reliable, and products get returned, wasted, or flagged for quality issues at different rates. Without pulling this information together, it's hard to quickly identify which suppliers, warehouses, or channels are underperforming — or how these operational problems are impacting revenue and profitability.

# What is this project about?

This project digs into real operational data to answer simple but important questions:

Are we delivering orders on time?
Where are we losing money — waste, returns, or stockouts?
Which suppliers and warehouses are underperforming?
How healthy is the overall supply chain, at a glance?

# Tools Used


Python (Pandas)	Cleaning the data and doing initial exploration (EDA)

PostgreSQL	Storing the data and running SQL queries

Power BI	Building the final interactive dashboard

## Dataset

The dataset covers 2 years of operations and includes:

2,200 orders — with delivery dates, quantities, prices, and flags for late delivery, stockouts, returns, waste, and quality issues

5,040 inventory snapshots — monthly stock levels across 5 warehouses and 42 products

Supporting details on 8 suppliers, 80 customers, 5 warehouses, and 42 products

# What I did
Cleaned and explored the data in Python — checked for missing values, fixed date formats, and looked at basic stats for every table.

Loaded the data into PostgreSQL and wrote 20+ SQL queries — from simple filters to joins, window functions, and CTEs — to answer real business questions.

Built a 3-page Power BI dashboard with KPIs, trend charts, and interactive filters to explore delivery performance, inventory risk, and supplier quality.

# Dashboard


The dashboard has 3 pages:

- Overview

The big picture — Revenue, Gross Profit, OTIF% (on-time-in-full delivery rate), and an overall "Supply Chain Health Score." Includes a chart showing exactly where profit is lost between Revenue and final profit (waste, returns, and costs).

![dashboard]()

- Delivery & Risk

Focuses on how reliably orders are delivered — which warehouses are slower, which customer types face more delays, and how much revenue is tied up in risky orders (late, out-of-stock, or quality issues).

![dashboard]()

- Supplier & Quality

Looks at the supply side — which suppliers are more reliable, which ones have higher defect rates, and where waste is happening across categories and warehouses.

![dashboard]()

# Key Insights

Dairy products lose the most profit to waste and returns — likely because they're perishable and don't last as long on the shelf.

One warehouse (Riga Central DC) accounts for the largest share of late deliveries — a good place to start fixing delivery problems.

Retail is the biggest revenue channel, but that doesn't automatically mean it's the most profitable — margin matters just as much as revenue.

A few suppliers combine lower reliability with higher defect rates — these are the ones worth watching most closely.

# Recommendations

Based on the analysis, here's what the business could do to improve:

Focus on Dairy first — since it has the highest margin leakage, look into better cold storage handling, shorter reorder cycles, or improved shelf-life tracking to cut down on waste and returns.

Fix delivery issues at Riga Central DC — this warehouse has the largest share of late orders, so improving its processes could have the biggest impact on overall on-time delivery.

Review supplier contracts for high-risk suppliers — suppliers with both low reliability and high defect rates should be monitored closely, or alternative suppliers should be considered.

Balance revenue with profitability across channels — don't just chase the channel with the highest revenue; check which channel actually keeps the most profit per sale.

Set clear targets and track them over time — using targets like "OTIF should stay above 95%" or "stockout rate should stay below 2%" helps turn raw numbers into clear, actionable goals.

# Conclusion

This project shows how raw supply chain data — orders, inventory snapshots, and supplier details — can be turned into clear, actionable insights using Python, SQL, and Power BI. Instead of just reporting numbers, the dashboard highlights where problems are happening (which category, which warehouse, which supplier) and why they matter to the business's bottom line.

The biggest takeaway is that small, everyday issues — a late delivery here, some wasted stock there — add up to a real, measurable impact on profit. By tracking these issues together in one place, a business can move from reacting to problems after they happen to catching and fixing them early.
