# Data-Analyst-Internship-Task-7

## Objective
To extract and visualize basic sales data using SQL queries inside Python.

## Tools Used
- Python
- SQLite (via sqlite3 module)
- Pandas
- Matplotlib
- Jupyter Notebook

## Steps Performed
1. Created a SQLite database (`sales_data.db`) and a table named `sales`.
2. Inserted sample product-wise quantity and price data.
3. Ran SQL query using pandas to get total quantity sold and revenue per product.
4. Displayed result in tabular format using print.
5. Visualized revenue by product using a matplotlib bar chart.

## Output
- `sales_chart.png` showing revenue for each product.

## How to Run
- Run the notebook step-by-step in Jupyter.
- Make sure `sales_data.db` gets created in your project folder.
- Chart will be saved as `sales_chart.png`.

## Sample SQL Query Used
```sql
SELECT product, SUM(quantity) AS total_qty, SUM(quantity * price) AS revenue
FROM sales
GROUP BY product;
