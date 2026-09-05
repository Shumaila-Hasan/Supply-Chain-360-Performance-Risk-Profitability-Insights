# Supply_Chain_FP20

# Food & Beverage Supply Chain Analytics

An end-to-end data analytics project that looks at how a food & beverage company manages its supply chain — from the moment an order is placed to the moment it's delivered. The project covers data cleaning, SQL analysis, and an interactive Power BI dashboard.

# What is this project about?

Companies that sell food and beverages deal with a lot of moving parts — orders, suppliers, warehouses, and customers across different channels (Retail, E-commerce, HoReCa, Distributors). Along the way, things can go wrong: deliveries arrive late, warehouses run out of stock, products expire, and some orders get returned.

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

- Delivery & Risk

Focuses on how reliably orders are delivered — which warehouses are slower, which customer types face more delays, and how much revenue is tied up in risky orders (late, out-of-stock, or quality issues).

- Supplier & Quality

Looks at the supply side — which suppliers are more reliable, which ones have higher defect rates, and where waste is happening across categories and warehouses.

# Key Insights

Dairy products lose the most profit to waste and returns — likely because they're perishable and don't last as long on the shelf.

One warehouse (Riga Central DC) accounts for the largest share of late deliveries — a good place to start fixing delivery problems.

Retail is the biggest revenue channel, but that doesn't automatically mean it's the most profitable — margin matters just as much as revenue.

A few suppliers combine lower reliability with higher defect rates — these are the ones worth watching most closely.
