# SQL Query Portfolio – Troy Farley

1. Total Sales by Region
```sql
SELECT Region, SUM("Total Revenue") AS total_sales
FROM sales_data
GROUP BY Region
ORDER BY total_sales DESC;
```

2. Monthly Sales Trend by Product
```sql
SELECT Product, Month, SUM("Units Sold") AS total_units
FROM sales_data
GROUP BY Product, Month
ORDER BY Product, Month;
```
