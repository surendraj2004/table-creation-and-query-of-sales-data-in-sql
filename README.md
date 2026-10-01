Sales Data Analysis Using SQL
Project Overview

This is a beginner-friendly SQL project using SQLite and Python. The project focuses on creating tables, inserting customer and order data, joining tables, and filtering sales information using SQL queries.

Tools and Technologies
SQL
SQLite
Python
Pandas
Jupyter Notebook
Project Objectives
Create customer and order tables
Understand primary keys and foreign keys
Insert sample customer and order data
Combine data from multiple tables using INNER JOIN
Filter data using WHERE conditions
Display SQL query results using Pandas
SQL Query Used
SELECT customers.name, customers.city, orders.amount
FROM customers
INNER JOIN orders
ON customers.customer_id = orders.customer_id
WHERE customers.city = "New York"
AND orders.amount > 100;
Result

The query identifies customers from New York whose order amount is greater than 100.

Name	City	Amount
John	New York	150
David	New York	120
What I Learned

Through this project, I learned the basics of working with relational data using SQL. I practiced creating tables, using primary and foreign keys, inserting data, joining tables, filtering records, and working with SQL results in Pandas.

Project Structure
sales_data_sql_analysis.ipynb
README.md
Author

Surendra J