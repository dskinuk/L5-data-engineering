# Advanced SQL

## Impacts of upstream data modelling on downstream experience

1. Data base Views - Saved SQL queries
2. Stored procedures - User created code snippet developed to perform a set of sql queries and lof=gical operations on one or multiple database tables/views.
3. CRUD - SQL and Data definition language statements.
    - C - Create/Insert
    - R - Read/Select
    - U - Update
    - D - Delete

## Importance of Good Data Modelling
  - Conceptual Data Model
    - Business Requirements
    - Business processes and rules
  - Logical Data Model
    - Data Types
    - Normalisation
  - Physical Data Model
    - Primary and Foreign Keys
    - Views
    - Indexes
  
    

## ACID and the importance of transacions
- ACID - Atomicity, COnsistency, Isolation, Durability

## Nested SQL queries 
- Nested Create - Create a table based on the result of a sub query. Helps create tables from existing tables.
- Nested Read - Displays data based on the subquery
- Nested Update - Allows an update to  the table data based on a subquery
- Nested Delete - Allows deletion of table data based on a subquery

Co-related subqueries
## Joins and Data Normalisation
- Inner Join - rows common in bothe tables are displayed
- Outer
    - left - All rows in left table and matching rows in right table
    - Right - All rows in right table and matching rows in left table
    - Full - All rows that do not match in left nad right tables
- Cross Join - For every row in left table match all rows in right table

### Normalisation - Addresses issues of redundancy and integrity by ensuring that data is tored only once thus eliminating anomalies.
- First Normal Form - All columns hold aromic values and each record is unique
- Second Normal Form - All non key attributes are fully dependent on the primary key
- Third Normal Form - No transitive dependecies between key and non key attributes

## Group By
Allows data aggregations i.e. grouping by order types and taking a sum of order amount

- Window Function 

SELECT Store_ID, 
       QUARTER(Sale_Date) AS Sale_Quarter,
       SUM(Sales_Amount) AS Total_Sales,
       AVG(Sales_Amount) AS Average_Sales,
       SUM(Sales_Amount) OVER (PARTITION BY Store_ID ORDER BY Sale_Quarter 
       ROWS BETWEEN 1 PRECEDING AND CURRENT ROW) AS Running_Total
FROM Sales
GROUP BY Store_ID, Sale_Quarter
ORDER BY Store_ID, Sale_Quarter;

## Risks and Disaster Recovery 
