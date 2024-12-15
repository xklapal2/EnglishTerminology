### Terminology

| **Term**                                    | **Explanation**                                              |
| ------------------------------------------- | ------------------------------------------------------------ |
| **Database**                                | A place where data is stored and managed for easy retrieval and processing. |
| Database Management System (DBMS)           | Software that manages databases, separating data from applications and providing functions like querying, updating, and data security. |
| Relational Database                         | A database model where data is organized into tables, and relationships are managed using primary and foreign keys. |
| Data                                        | Raw, unprocessed facts such as numbers, letters, or symbols. |
| Information                                 | Processed and structured data that is useful in a given context. |
| Knowledge                                   | Organized information that helps in decision-making and understanding. |
| Data Model                                  | A description of the structure of data in a database, including relationships and access methods. |
| Concurrency                                 | The ability of a database to handle multiple operations simultaneously. |
| Data Integrity                              | Ensuring accuracy and consistency of data over its lifecycle. |
| **Modelling and design**                    |                                                              |
| **Logical Data Model**                      | Identifies necessary data, their relationships, and how they are grouped, based on the information needs of an organization. |
| Entity                                      | An object or concept about which data is stored (e.g., customer, product). |
| Attribute                                   | Another term for a field or column in a table.               |
| Relationship                                | A connection between two entities in a database.             |
| **Physical Data Model**                     | Focuses on how data is physically stored in a database system, including storage and efficiency considerations. |
| Entity-Relationship (ER) Model              | A diagram that represents entities and their relationships in a database. |
| Normalization                               | The process of organizing data to reduce redundancy and improve data integrity. |
| Normalization Forms (1NF, 2NF, 3NF)         | Different levels of database normalization used to reduce redundancy. |
| Data Redundancy                             | The unnecessary repetition of data across multiple tables or locations. |
| Table                                       | A set of data elements arranged in rows and columns within a database. |
| Record (Row)                                | A single, complete entry in a table (one row of data).       |
| Field (Column)                              | A single piece of data within a record, like a category or property. |
| Primary Key                                 | A unique identifier for each record in a table.              |
| Composite Key                               | A primary key made up of more than one column.               |
| Foreign Key                                 | A field that establishes a relationship between two tables by referencing the primary key of another table. |
| Index                                       | A data structure that improves the speed of data retrieval operations. |
| Optionality/Nullable (Mandatory - opposite) | Defines if attribute must have a value.                      |
| Cardinality                                 | Defines the relationship between entities (e.g., one-to-one, one-to-many, many-to-many). |
| Intersection table                          | Table that solves many-to-many relationship.                 |
| Constraint                                  | A rule applied to a column to enforce data integrity (e.g., NOT NULL). |
| Data Type                                   | Specifies the kind of data (e.g., integer, string) that can be stored in a field. |
| NULL                                        | A special marker used to indicate that a field has no value. |
| BLOB (Binary Large Object)                  | A data type used to store large binary objects like images or videos. |
| Schema                                      | The structure of a database, including tables, relationships, and fields. |
| **SQL (Structured Query Language)**         | A programming language used to manage and manipulate databases. |
| Relational Algebra                          | A theoretical foundation for SQL operations, based on set theory. |
| Query                                       | A request to retrieve data from a database, often written in SQL. |
| Projection                                  | An operation in SQL that retrieves specific columns from a table. |
| Selection                                   | An operation that retrieves specific rows from a table based on a condition. |
| Join                                        | Combining rows from two or more tables based on a related column. |
| View                                        | A virtual table based on the result of a query.              |
| Transaction                                 | A set of operations that are treated as a single unit of work. |
| Commit                                      | Permanently saving changes from a transaction to the database. |
| Rollback                                    | Reversing changes made by a transaction before they are committed. |
| Aggregation                                 | Operations that calculate summary values (e.g., SUM, AVG, COUNT). |
| Backup                                      | A copy of data stored separately for recovery purposes.      |
| Restore/Recovery                            | The process of returning data to a previous state using a backup. |
| **SQL subsets**                             |                                                              |
| DML (Data Manipulation Language)            | A subset of SQL used to insert, update, delete, and query data. |
| DDL (Data Definition Language)              | A subset of SQL used to define database structures (e.g., CREATE, ALTER). |
| DCL (Data Control Language)                 | A subset of SQL used to control access to data (e.g., GRANT, REVOKE). |
| TCL (Transaction Control Language)          | A subset of SQL used to manage transactions (e.g., COMMIT, ROLLBACK). |
| **Other**                                   |                                                              |
| Replication                                 | Copying data between multiple databases to ensure consistency and redundancy. |
| Sharding                                    | Splitting a large database into smaller, more manageable parts. |
| Deadlock                                    | A situation where two or more processes are stuck waiting for each other to release resources. |
| Cluster                                     | A set of databases or servers working together as a single system. |
| Partition                                   | Dividing a table into smaller pieces to improve performance. |
| Data Mining                                 | The process of analyzing large data sets to discover patterns or insights. |

### 4. **Typical Database Operations**

The e-shop will rely on several common database operations to support its functionality:

- **Checking Stock Levels**: The system queries stock levels in real-time, ensuring that customers cannot purchase products that are out of stock. This is crucial for maintaining accurate inventory records and preventing overselling, especially during peak shopping times or promotional events.

  **Retrieving Customer Orders**: Customers can easily access their order history, which includes information such as products purchased, quantities, payment status, and shipping details. This not only enhances customer service but also allows the system to track buying behavior over time.

  **Generating Reports**: Database systems allow admins to generate detailed reports on various aspects of the business, such as sales performance, customer preferences, inventory status, and order histories. These reports provide critical insights into what customers are purchasing and what products are searched for the most. Analyzing this data helps the business identify popular items, peak buying times, and customer trends.

  By understanding customer behavior, the e-shop can tailor its product offerings more effectively. For example:

  - **Enhanced Offers**: Reports on frequently purchased products or items often searched by customers allow the system to suggest personalized recommendations and special offers. By promoting related or complementary products based on previous purchases, the e-shop can increase cross-selling and up-selling opportunities.
  - **Targeted Marketing**: Insights gained from these reports can inform marketing strategies, such as creating targeted email campaigns or product bundles that cater to customers' preferences.
  - **Stock Optimization**: Reports can help identify products with high demand, enabling the store to restock them more efficiently while avoiding overstocking less popular items.

These operations will be optimized for performance, especially during peak traffic periods like sales seasons.

### 5. **Common Functional Requirements**

#### a) **Product Catalog Management**

The database must support adding, modifying, and deleting products. Products should be categorized (e.g., electronics, wearables, phones), and each category must have specific attributes like brand, price, and features. The system can be designed to include a **Category** table linked to the **Product** table for flexibility in product grouping and filtering.

#### b) **Inventory Management**

Stock levels are tracked within the **Product** table. Automated alerts will be generated when stock levels fall below a predefined threshold. This functionality can be achieved by setting up triggers or scheduled tasks within the database.

#### c) **Customer Management**

The **Customer** entity stores all user information, and a separate **Order** table will store customer orders. User registration and login processes will securely store hashed passwords, and each customer profile will link to past orders.

#### d) **Order Processing**

When a customer places an order, it updates both the **Order** table and the **Product** table (to reduce stock levels). Payment and shipping details are also recorded.

#### e) **Search and Filter Functionality**

Search and filtering can be achieved using SQL queries that retrieve products based on keywords (e.g., product name, description) or filters (e.g., price range, brand). Indexing key columns like product name and price will optimize these queries for performance.

#### f) **Recommendation System**

A recommendation system can be built by analyzing the **Order** and **Customer** tables. By examining past purchases or browsing behaviors, the system can suggest relevant products to each customer.

#### g) **Analytics and Reporting**

The database will enable the generation of reports on sales performance, popular products, and customer behavior. The database's aggregation functions will play a key role in summarizing this data for decision-making.

#### h) **Security and User Authentication**

The database must support secure user authentication, encrypting sensitive information such as passwords and payment data. SQL injection prevention mechanisms (e.g., using prepared statements) will safeguard against common vulnerabilities.

### 6. **Non-functional Requirements**

#### a) **Scalability**

The database must be scalable to handle growing user traffic, especially during promotions or high-demand periods. Vertical scaling (upgrading hardware) or horizontal scaling (database sharding) may be required as the user base expands.

#### b) **Performance**

The database must perform efficiently, even during peak usage. Techniques like query optimization, indexing, and database caching can help maintain quick response times.

#### c) **Reliability**

The system must guarantee high availability (99.9% uptime) through measures like database replication and regular backups to prevent data loss.

#### d) **Security**

Encryption will be applied to sensitive data, such as payment details. Compliance with regulations like the General Data Protection Regulation (GDPR) ensures user privacy and data protection.

#### e) **Usability**

The database structure should facilitate easy interaction with the system, both for users making purchases and for administrators managing the catalog or running reports.

### Conclusion

A well-designed database is central to the functionality of an e-shop. By organizing product data, customer profiles, and order details efficiently, the system can provide seamless operations such as inventory management, order processing, and report generation. Prioritizing scalability, security, and performance ensures the e-shop is ready to meet both current and future demands while maintaining high levels of user satisfaction and data protection.