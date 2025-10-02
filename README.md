# Get-Basic-Sales-Summary-from-a-Tiny-SQLite-Database-using-Python
Here is Get Basic Sales Summary from a Tiny SQLite Database which has been done in Jupyter Notebook using python

#Steps Performed
#Dataset Preparation

Started with a small sales dataset (sales_task7.csv / .xlsx).
Cleaned and standardized columns (product, quantity, price, order_date).

#Database Creation
Created a local SQLite database file: sales_data.db.
Added a sales table and inserted the dataset.

#SQL Queries
Aggregated per-product totals:
SELECT product,
       SUM(quantity) AS total_qty,
       SUM(quantity * price) AS revenue
FROM sales
GROUP BY product
ORDER BY revenue DESC;
Calculated overall totals (all products combined).

#Results
Printed per-product summary (total quantities & revenues).
Printed overall totals.

#Visualization
Plotted Revenue by Product as a bar chart.
Saved chart as sales_chart_task7.png.

#Outcome
Learned how to connect Python with SQLite.
Practiced SQL aggregation queries (SUM, GROUP BY, ORDER BY).
Imported SQL query results into Pandas DataFrame.
Generated and saved a simple bar chart visualization.
