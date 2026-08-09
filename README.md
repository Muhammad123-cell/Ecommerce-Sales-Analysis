# Ecommerce Sales Analysis

A Power BI dashboard built to analyze e-commerce order data for a retail store, covering sales, profit, product performance, regional trends, customer behavior, and payment methods for the year 2018.

![Ecommerce Sales Dashboard](Ecommerce_Sales_Dashboard.png)

## Project Files

| File | Description |
|---|---|
| `Capstone_Project.pbix` | Power BI dashboard file |
| `Orders.csv` | Order-level data: Order ID, Order Date, Customer Name, State, City (500 records) |
| `Details.csv` | Product/transaction-level data: Order ID, Amount, Profit, Quantity, Category, Sub-Category, Payment Mode (1,500 records) |
| `Ecommerce_Sales_Dashboard.png` | Screenshot of the final dashboard |

The two datasets are joined on the common field `Order ID`.

## Business Problem

The company generates large volumes of e-commerce order data, but had no centralized, visual way to interpret it. Management lacked clear visibility into overall sales performance, profitability drivers, underperforming products or regions, and customer purchasing behavior. This made it difficult to take data-driven decisions on inventory, marketing, and regional strategy.

## Objectives

- Consolidate order and product-level transaction data into a single, unified data model
- Track core KPIs: Total Sales, Total Profit, Total Quantity Sold, and Average Order Value
- Analyze profitability across product categories and sub-categories
- Evaluate regional performance across states
- Identify top customers by revenue
- Understand payment behavior across payment modes (COD, UPI, Card, EMI)
- Monitor sales and profit trends over time to detect seasonality
- Enable interactive, self-service exploration through filters and slicers (date and state)

## Key Performance Indicators (KPIs)

- **Total Sales** - Sum of Amount
- **Total Profit** - Sum of Profit
- **Total Quantity Sold** - Sum of Quantity
- **Average Order Value** - Amount divided by number of orders

Segmented across: Month, Sub-Category, Category, Payment Mode, State, and Customer.

## Key Business Insights

1. Overall profit margin is thin at roughly 8.4 percent (Total Sales: 4,37,771; Total Profit: 36,963)
2. Furnishings and Electronic Games sub-categories are running at a net loss despite meaningful sales volume
3. Furniture is the weakest-performing category overall, pulled down by Furnishings
4. Cash on Delivery (COD) accounts for the largest share of transactions, creating cash-flow and return risk
5. Credit Card is the most profit-efficient payment channel per rupee of sales
6. Maharashtra and Madhya Pradesh together account for over 43 percent of total sales, indicating geographic concentration
7. The top customer by revenue (Harivansh) is actually unprofitable due to discounting or returns
8. Profit shows strong seasonality, with Q1 and November performing best, and a mid-year (Q2-Q3) dip into losses

## Recommendations

- Review pricing and discounting for loss-making sub-categories (Furnishings, Electronic Games)
- Reduce dependence on COD by incentivizing prepaid payment methods
- Diversify sales beyond Maharashtra and Madhya Pradesh into other states
- Track customer-level profitability, not just revenue, before applying discounts
- Investigate the root cause of the Q2-Q3 profit dip
- Extend the strong Q4/November performance into December through targeted campaigns
- Promote high-margin sub-categories such as Printers, Bookcases, and Saree

## Conclusion

The dashboard shows a business generating solid revenue but converting very little of it into profit. Breaking performance down by product, payment mode, geography, customer, and time reveals exactly where margin is being lost, shifting the analysis from "are we profitable" to "where are we profitable and where are we losing margin." Acting on the recommendations above can improve profitability without necessarily growing total sales.

## Tools Used

- Power BI Desktop for data modeling, DAX measures, and dashboard visualization
- CSV source files for order and product/transaction data
