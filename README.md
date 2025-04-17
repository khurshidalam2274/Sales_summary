# Sales_summary
# Task 7 – Sales Summary (Data Analyst Internship)

This project demonstrates how to:
- Create and query an SQLite database using Python
- Use SQL to summarize sales data
- Visualize the results using Matplotlib

## 🛠 Tools Used:
- Python
- SQLite (via `sqlite3`)
- Pandas
- Matplotlib
- VS Code

## 📊 Output:
- Total quantity and revenue by product
- A bar chart saved as `sales_chart.png`

## 💻 How to Run:
1. Clone the repo or download the files
2. Run `task7_sales_summary.py` using any Python environment (VS Code recommended)
3. See printed summary in terminal and the saved bar chart

## 📌 SQL Query Used:
```sql
SELECT product, 
       SUM(quantity) AS total_quantity, 
       SUM(quantity * price) AS total_revenue
FROM sales
GROUP BY product;
