# NO SQL Fundamentals

## DIscovering MongoDB
Among the various types of NoSQL databases available such as key-value, wide-column, document, and graph databases, MongoDB—a document-oriented database. It has 
  - Flexible schema
  - Scalability
  - Robust querying capabilities
  - A JSON like document model
  - An ability to handle large volumes of unstructured and semi-structured data

### Strcuture of MomgoDB database
  Stores data in 
  
    - Collections - Similar to Tables, colleactions hold documents and does not require them to have the same schema
    - Documents - Consists of Key Value PAirs and are the absic unit storage of the DB. Similar to rows in a table, but can contain data of any type or structure.

### Extracting data from MongoDB
- Scraping web pages
- Parsing texts
- Interfacing with API s
- Reading Meta Data

### Transforming unstructured data
- Data Quality - Unstructured data can be messy. Use data cleaning tools/libraries like pandas
- Computational Intensity - Processes like sentiment analysis ca be resource heavy. Use efficient algorithms
- Evolution of data - transformation process might need updates as data grows. Regularly review the logic and maintain code.

### Transitioning MongoDB to SQL
MongoDB, a NoSQL database, offers flexibility in handling diverse and evolving data structures.

However, when data maturity reaches a point, or structured querying and analysis are required, SQL databases become indispensable.

- Evaluation
- Transformation
- Migration
- Validation
- Optimisation
- COntinuos Sync

Unstructured data sources => Transform using Pyhton Libs => Semi structured MongoDB => Transform to Rel DB => Input into SQL => SQL DB

    
