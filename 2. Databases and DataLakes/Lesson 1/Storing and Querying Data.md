# Storing files 
## HDFS, Key Value Store,Parquet files


1. Hadoop Distributed File System
  - Innovative approach for cheap commodity storage
  - Offers resilience by storing multiple copies of each file in different locations
    
2.  Key-Value Stores
  - Aggregations on a per key basis
  - Each key corresponds to a umique identifier associated with a specific data entry
  - Popular datasets - Redis, Riak, Berkeley DB, Memcached, Amazon DynamoDB, Azure Cosmos DB, Google Cloud BigTable
  - Cached data like user session management data, shopping cart contents
  - Real time analytics, Content ,management systems, Product catalogs 
    
3. Parquet files
  - Files are coulmnar storage formats
  - This structure allows for better compression and efficient storage especially for large datasets with many columns

## Data Lakes, Data Ware Houses and Operational Data Stores

1. Data Lakes - Unstructured Data Haven, they are vast reservoirs of unstructured data capturing everything from logs, XML files to social mdeia posts. They provide flexibility in data storage allowing storage in native format without the need of an upfrint schema definition.
2. Data Warehouses - Highly structured reositories designed to facilitate efficient data analysis and reporting. Essential for businesses who rely on hstorical data analysis to inform strategic decison making.
3. ODS  Operational data Store - Real time data processing of transactional data supporting day to day business operations.

## Data Structuring: Schema-on-Write, Relational Modelling

1. Schema-on-Write - Requires Scheme to be defined before writing data to the database


2. Relational Modelling - Method used to structure data in a database by defining relationships among data points.
  - Organises data in tables (relations) that include rows(tuples) and columns(attributes).
  - Primary Key and Foreign Key relationships
  - every elemnet has a specific place and relation to others
  - enabling easy navigation and management

## Storing Data on Cloud Vs On Premise
1. On Premise
   - Maintaining data servers and infrastructure within the physical premise
   - complete control of data environments including security protocols and access mechanism
   - best suited for high security requirements or those that handle sensitive data where regulatory comliance is paramount
  
2. CLoud Solution
  - Hosting data on servers managed by 3rd party providers accessible on the internet
  - offers flexibility, scalability and cost efficient
  - can Pay as you go
  - best suited for organisations looking for operational flexibility, cost savings and ability to scale quickly. 
  -  
   
