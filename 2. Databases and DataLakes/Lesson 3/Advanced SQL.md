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
Nested Create
Nested Read
Nested Update
Nested Delete

Co-related subqueries
## Joins and Data Normalisation
- Inner Join
- Outer (left, Right, Full)
- Cross Join

### Normalisation - Addresses issues of redundancy and integrity by ensuring that data is tored only once thus eliminating anomalies.
- First Normal Form - All columns hold aromic values and each record is unique
- Second Normal Form - All non key attributes are fully dependent on the primary key
- Third Normal Form - No transitive dependecies between key and non key attributes

## Group By

## Risks and Disaster Recovery 
