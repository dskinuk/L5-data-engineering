# Data Base Administartion and Optimisation

## Database administrtaion Best Practices
  - Choosing the right Database management system - The data structure and its relationships
      - Scalability - Expected Data volume and growth
      - Performance - Query patterns and performance expectations
      - Data Consistency - Consistency and available trade offs.
      - Transaction

        Partitioning and sharding techniques distribute data across multiple nodes or servers, either through horizontal partitioning (sharding) based on a key or range or vertical partitioning based on columns or data types. This improves query performance and scalability. Caching mechanisms, such as implementing caching layers (e.g., Redis, Memcached) and storing frequently accessed data in memory, reduce database load and improve response times. Regular monitoring of database metrics, identifying performance bottlenecks and slow queries, tuning database parameters and configurations, and analysing and optimising query execution plans are essential for maintaining optimal performance.
## Database Security
- Authorisation and Access control
- Authentication
- Data encryption
- Data Integration and Verification
- Data Privacy Protection
- Auditing and Logging

## SQL and NOSQL databases

- SQL databases
    - Structure data in tables with rows and columns
    - Data relationships through Primary and Foreisgn keys
    - Normalization of data
    - Use Structured Query Language
    - Can Create, ALter Drop tables and manipulate table data by Insert, Update, Delete
    -  Examples include financial systems, e-commerce platforms, and content management systems. 
- NO SQL (Not only SQL) Databases
    - For large volumes of unstructured or semi structured data
    - non relational data models such as Key Value stores, document databases (JSON/XML)
    - Offer flexible schema allowing for dynamic and evolving data structures(schema less or schema on Read approach)
    - designed for horizontal scalability across multiple servers
    - NoSQL databases often prioritise eventual consistency, relaxing strict consistency in favour of availability and partition tolerance. This allows for temporary inconsistencies that are eventually resolved, making them suitable for applications that can tolerate eventual consistency.
    - Examples include social networks, real-time analytics, and content delivery networks.
## Monitoring and Optimising Database performance
- Monitoring metrics
    - Response time
    - Throughput
    - Concurrency
    - resource utilisation
    - Indexing
 
- Tools
    - Query Profiling
    - Indexing Strategies
    - DB Config
 
      
