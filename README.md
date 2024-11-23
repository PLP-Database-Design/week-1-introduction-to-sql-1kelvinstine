# SQL Assignment Week 1


## *What You'll Need*
- A computer with internet access.
- A code editor (e.g., Visual Studio Code).
- MySQL Workbench or another SQL database environment.

---



## *Submission Instructions*
1. Answer every question below and put your responses in a file named `answers.md`
2. Push your completed `answers.md` file to your GitHub repository.
3. Submit the GitHub link for review.

---

## **Assignment Questions**

# 1. State and Explain the components of a DBMS(Database Management System)
 .1. Hardware
Description: The physical devices used to store and run the DBMS.
Examples: Servers, storage devices, and network infrastructure.
Function:
Provides the computational power to process data.
Stores the database and supports system operations.

2.Software
Description: The set of programs that manage and operate the database.
Key Layers:
DBMS Software: Core system for managing databases (e.g., MySQL, Oracle DB).
Operating System: Manages underlying hardware resources.
Application Programs: Interfaces that connect users to the DBMS.
Function:
Provides tools for database definition, access, and management.
Implements user queries and operations.
3.Data

Description: The collection of raw information stored in the database.
Types:
User Data: Data inserted by users, such as employee records or sales data.
Metadata: Data about data (e.g., schemas, table structures, constraints).
Indexes: Structures to enhance query performance.
Function: Forms the core of the DBMS; it is organized for efficient retrieval and modification.

4.Users
Description: Individuals or applications that interact with the DBMS.
Categories:
Database Administrators (DBAs): Configure and maintain the DBMS.
Developers: Design applications and interact with the database via APIs.
End Users: Access and manipulate data through applications.
Function: Utilize the database for various operations like querying, reporting, and transaction management.

5.Query Processor
Description: The component that interprets and executes database queries.
Sub-components:
DDL Compiler: Processes Data Definition Language (DDL) commands (e.g., CREATE TABLE).
DML Compiler: Processes Data Manipulation Language (DML) commands (e.g., SELECT, INSERT).
Query Optimizer: Enhances query performance by generating efficient execution plans.
Function: Converts high-level queries into low-level instructions for execution.

6).Database Engine
Description: The core service that processes and manages database operations.
Function:
Executes query plans.
Ensures data consistency and integrity through transaction management.
Manages concurrent access to the database.

7).Data Dictionary
Description: A metadata repository that stores information about database structure and rules.
Contents:
Table names, column data types, constraints, and relationships.
Function:
Helps enforce database integrity.
Provides a reference for the DBMS to process queries and updates.

8).Transaction Management
Description: Ensures database consistency during multiple operations (transactions).
Key Features:
ACID Properties: Atomicity, Consistency, Isolation, Durability.
Concurrency Control: Manages simultaneous operations.
Function: Guarantees reliability and integrity in multi-user environments.

9).Communication Interfaces
Description: Mechanisms for users and applications to interact with the DBMS.
Examples:
Graphical User Interfaces (GUIs): Simplified tools for end-users.
APIs: Programming interfaces for developers.
Command-Line Interfaces (CLIs): Direct interaction via commands.
Function: Facilitates user-friendly and programmatic access to the database.
# 2. What is a relational database? Give 4 examples.
 A relational database is a type of database that stores data in a structured format, using rows and columns organized into tables. 
 
 Each table represents a specific entity (e.g., customers, products) and includes attributes (columns) that describe the entity's properties. 


Relationships between the tables are established using keys, such as primary keys and foreign keys.

The relational model is based on relational algebra and ensures data integrity, consistency, and easy querying using a standard language called SQL (Structured Query Language).

# 3. State and Explain three classifications of SQL?
 a)Data Definition Language (DDL)
Description:
DDL statements are used to define, modify, and manage the structure of database objects like tables, schemas, and indexes.

b)Data Manipulation Language (DML)
Description:
DML statements handle data manipulation tasks, such as inserting, updating, retrieving, or deleting data within database tables

 c).Data Control Language (DCL)
Description:
DCL statements manage access permissions and control privileges for database objects. 



# 4. What is the difference between a Primary Key and a Foreign Key?
 1).Primary Key
Definition:
A primary key is a unique identifier for a record (row) in a table. It ensures that each record is distinct and can be uniquely identified.

Characteristics:

Uniqueness: Each value in the primary key column must be unique.

Non-Null: A primary key column cannot have NULL values.

Single or Composite: Can consist of a single column or a combination of columns (composite key).

Exists Within a Table: Defined within a single table to identify rows uniquely.

 2).Foreign Key
Definition:
A foreign key is a column (or set of columns) in one table that establishes a link to a primary key in another table. It is used to enforce relationships between tables.

Characteristics:

References Another Table: The foreign key references the primary key in another table (or the same table in a self-referencing relationship).

Allows Null or Duplicate Values: A foreign key column may contain NULL values (if allowed) and can have duplicate values.

Ensures Referential Integrity: Prevents invalid data by ensuring that the value in the foreign key column matches a value in the referenced table's primary key.

# 5. What is an Entity-Relationship Diagram?
An Entity-Relationship Diagram (ERD) is a graphical representation of the entities, attributes, and relationships within a database system. 

It is a critical design tool used in database modeling to visually depict how data is organized and how different entities are related to one another.

# 6. What are the advantages of relational databases?
 1.Simplicity
Explanation: Relational databases organize data in a tabular format, which is intuitive and easy to understand.

Advantage: Users can interact with the data without needing extensive technical knowledge, using tools like Structured Query Language (SQL).

2).Flexibility
Explanation: Relational databases can adapt to changing requirements by adding, modifying, or removing tables, columns, and relationships.
Advantage: They support evolving business needs without significant restructuring.

3).Data Integrity and Accuracy
Explanation: Enforces constraints (e.g., primary keys, foreign keys, unique constraints) to ensure the validity and consistency of data.
Advantage: Minimizes errors and ensures reliable data.

4).Data Security
Explanation: Relational databases offer robust access controls, allowing administrators to define who can view or modify data.
Advantage: Ensures sensitive data is protected against unauthorized access.
5).Scalability
Explanation: Relational databases are designed to handle large amounts of data efficiently and can scale vertically (improving hardware) or horizontally (adding more servers).
Advantage: Suitable for both small applications and enterprise-level systems.


# 7. State four types of data type used to store data in tables?
 1.Integer (Numeric Data Types)
Purpose: Stores whole numbers.

Examples:
INT: A standard integer.

BIGINT: A larger range of integers.

SMALLINT: A smaller range of integers.

Use Case: To store values like IDs, counts, or quantitie

 2).Decimal/Float (Numeric with Decimal)
Purpose: Stores numbers with decimal points.

Examples:

DECIMAL(p, s) or NUMERIC: Precise numeric data with a fixed number of decimal places.

FLOAT or REAL: Used for approximate decimal values.

Use Case: To store monetary values or measurements (e.g., weight, height).
 3).String (Character Data Types)
Purpose: Stores text or alphanumeric data.

Examples:

VARCHAR(n): Variable-length strings up to n characters.

CHAR(n): Fixed-length strings of n characters.

TEXT: Large amounts of text data.

Use Case: To store names, descriptions, or addresses

 4).Date/Time Data Types
Purpose: Stores dates and/or times.

Examples:

DATE: Stores a date (YYYY-MM-DD).

TIME: Stores time (HH:MM:SS).

DATETIME or TIMESTAMP: Stores both date and time.

Use Case: To store timestamps, order dates, or event schedules
   
# 8. What is the purpose of a database management system (DBMS)?  
 Data Storage and Organization

Purpose: To store data in an organized manner using tables, rows, and columns.

Why It Matters: Helps in systematic data retrieval and prevents redundancy or inconsistencies.

Data Retrieval

Purpose: To allow users or applications to query the database to fetch specific data.

Why It Matters: Simplifies complex data retrieval through SQL and supports data-driven decision-making.

Data Manipulation

Purpose: To add, update, delete, or modify data in the database.

Why It Matters: Ensures that data remains relevant and up-to-date for various operations.
Data Security

Purpose: To protect data from unauthorized access or malicious activity.

Why It Matters: Prevents data breaches and ensures sensitive data is accessed only by authorized users.

Examples: Role-based access control, encryption.
Data Integrity

Purpose: To ensure the accuracy, consistency, and reliability of data.

Why It Matters: Prevents errors, duplicates, or inconsistencies across database entries.

Examples: Use of constraints like primary keys, foreign keys, and validation rules.
Concurrency Control

Purpose: To enable multiple users to access and manipulate data simultaneously without conflicts.

Why It Matters: Ensures smooth operation in multi-user environments and maintains data consistency.

Backup and Recovery

Purpose: To provide mechanisms for backing up data and restoring it in case of failure.

Why It Matters: Ensures business continuity and prevents data loss during hardware or software failures.

Data Independence

Purpose: To separate the database structure from the application programs.

Why It Matters: Allows applications to evolve independently without affecting the underlying database schema.

Support for Data Relationships

Purpose: To manage relationships between data efficiently (e.g., one-to-many, many-to-many).

Why It Matters: Simplifies querying and ensures data integrity in relational databases.
Efficient Data Handling

Purpose: To optimize data storage and retrieval for speed and scalability.

Why It Matters: Enhances application performance and supports growing data volumes.


