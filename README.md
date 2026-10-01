# Sales Data Analysis Using SQL

## Overview

This project focuses on working with customer and order data using SQL and SQLite. It demonstrates how relational tables can be created, connected, queried, and analyzed using Python and Pandas.

The project uses two related tables, `customers` and `orders`, and applies SQL queries to combine and filter the data.

## Objectives

* Create relational tables using SQLite
* Define primary and foreign keys
* Insert customer and order data
* Combine data using `INNER JOIN`
* Filter records using `WHERE`
* Retrieve and display query results using Pandas

## Technologies Used

| Technology       | Purpose                                  |
| ---------------- | ---------------------------------------- |
| Python           | Data processing and database interaction |
| SQL              | Querying and analyzing data              |
| SQLite           | Database management                      |
| Pandas           | Reading and displaying query results     |
| Jupyter Notebook | Project development and execution        |

## Database Structure

### Customers Table

Stores customer information such as:

* Customer ID
* Customer Name
* City

### Orders Table

Stores order information such as:

* Order ID
* Customer ID
* Order Amount

The `customer_id` connects the two tables using a foreign key relationship.

## SQL Analysis

The project uses an `INNER JOIN` to combine customer and order information and applies filtering conditions to identify relevant sales records.

```sql
SELECT customers.name, customers.city, orders.amount
FROM customers
INNER JOIN orders
ON customers.customer_id = orders.customer_id
WHERE customers.city = "New York"
AND orders.amount > 100;
```

## Result

The query identifies customers from New York whose order amount is greater than 100.

| Name  | City     | Amount |
| ----- | -------- | -----: |
| John  | New York |    150 |
| David | New York |    120 |

## Key Concepts Covered

* Database and table creation
* Primary keys
* Foreign keys
* Data insertion
* INNER JOIN
* WHERE clause
* SQL result handling with Pandas

## Project Structure

```text
table-creation-and-query-of-sales-data-in-sql/
│
├── sales_data_sql_analysis.ipynb
├── README.md
│
└── images/
    ├── result1.png
    ├── result2.png
    └── result3.png
```

## Learning Outcome

This project provided practical experience in working with relational data and understanding how SQL can be used to connect and filter information stored across multiple tables.

## Author

Surendra J
