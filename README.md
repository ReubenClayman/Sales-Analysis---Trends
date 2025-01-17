Sales Analysis - Advanced Monthly Sales Trends with Growth Rate and Cumulative Sales

Objective: To perform a detailed analysis of sales trends over the past year, identifying monthly trends, seasonal patterns, overall growth or decline, and calculating cumulative sales and growth rates.

Tables/Columns Used:
sales (columns: sale_date, amount, region_id, product_id)
products (columns: product_id, product_name)
regions (columns: region_id, region_name)

Explanation:
Common Table Expressions (CTEs) are used to create intermediate results. The monthly_sales CTE aggregates sales data by month and region, and calculates the rank of regions by total sales.
Window Functions:
RANK() is used to rank regions based on their sales.
SUM() OVER() is used to calculate the cumulative sales for the year.
LAG() is used to compute the growth rate by comparing the current month's sales with the previous month's sales.
The final output shows monthly sales trends, cumulative sales, growth rate, and region ranks.
