Collection - 
 - [Datacamp](https://www.datacamp.com/blog/top-sql-interview-questions-and-answers-for-beginners-and-intermediate-practitioners)
 - [Interviewbit](https://www.interviewbit.com/sql-interview-questions/)
 - [Simplelearn](https://www.simplilearn.com/top-sql-interview-questions-and-answers-article)
 - [Roadmap.sh](https://roadmap.sh/questions/sql)
 - [Geeksforgeeks](https://www.geeksforgeeks.org/sql/sql-interview-questions/)
 - [wecreateproblems](https://www.wecreateproblems.com/interview-questions/sql-interview-questions)
 - [SQL practice](https://youtu.be/nYmoQ4r0DVw?si=eUxWJ8rzXRZC8V05)

- **What are SQL dialects? Give some examples.**
  - The different versions of SQL which syntax is slightly different, Like - PostgreSQL, MySQL etc.

- **What types of SQL commands do you know?**
  - Data Definition Language (DDL) - To change the structure of a database, like - CREATE, ALTER TABLE, DROP, TRUNCATE, and ADD COLUMN.
  - Data Manipulation Language (DML) - To modify data in a database, like - UPDATE, DELETE, and INSERT
  - Data Control Language (DCL) – To control user access in database and give or revoke privileges to a specific user or a group of users, like - GRANT and REVOKE.
  - Transaction Control Language (TCL) - To control transactions in database, like - COMMIT, SET TRANSACTION, ROLLBACK, and SAVEPOINT.
  - Data Query Language (DQL) – To retrieve information from database, like - SELECT.

- **What is a database?**
  - A structured storage space where the data is kept in many tables and organized so that the necessary information can be easily fetched, manipulated, and summarized.

- **What is DBMS, and what types of DBMS do you know?**
  - DBMS stands for `Database Management System`, a software package to perform various operations, like - accessing, changing, adding, removing data. There are different types of DBMS, like - relational, hierarchical, network etc. These types are the way how data is organised, structured and stored in the system.
  
- **What is RDBMS?**
  - RDBMS stands for `Relational Database Management System`. It is a type where data stored in multiple tables and connected with different types of keys. Examples are - MySQL, PostgreSQL etc.

- **What types of SQL subqueries do you know?**
  - Single-row – returns at most one row.
  - Multi-row – returns at least two rows.
  - Multi-column – returns at least two columns.
  - Correlated – a subquery related to the information from the outer query.
  - Nested – a subquery inside another subquery.

- **What is a constraint, and why use constraints?**
  - Constraint is a set of conditions by which input can be validated. Constraints ensure data integrity in a table and block undesired actions. Different constraints are - 
    - DEFAULT – provides a default value for a column.
    - UNIQUE – allows only unique values.
    - NOT NULL – allows only non-null values.
    - PRIMARY KEY – allows only unique and strictly non-null values (NOT NULL and UNIQUE).
    - FOREIGN KEY – provides shared keys between two or more tables.
    - SUPER KEY - 
    - COMPOSITE KEY - 

- **What is a join? What types of joins do you know?**
  - Inner join - returns the records that satisfy in both tables. It is a default SQL join. 
  - Left join - returns all records from the left table, and those records from the right table that satisfy a defined join condition. 
  - Right join - returns all records from the right table, and those records from the table that satisfy a defined join condition.
  - Full join - returns all records from both tables. No condition is applied here. It is a combination of left and right joins.

- **What is a primary key?**
  - It is a column (or combination of multiple columns) of a table to which `PRIMARY KEY` constraint is imposed to ensure unique and non-null values in that column. It uniquely identifies each record of the table. It is combination of `NOT NULL` and `UNIQUE` constraint. There can be only one primary key per table.

- **What is a unique key?**
  - This constraint ensures unique value in a column (or multiple columns). Interestingly `NULL` is allowed here but only once. Because NULL is also a value.

- **What is foreign key?**
  - This constraint is used to connect a table's column (or multiple columns) to other table's primary key's column. 

- **What is an index?**
  - A special data structure related to database table which is used for faster data search and retrieval. Indexes are efficient for large databases where it significantly enhances query performance. It does not do full-table-scan but goes into its own structure to find out the data. It uses B tree or B+ tree which is a balanced binary tree to store the index. As it is binary tree, so retrieval information is very fast. But the problem is when trying to update, delete or inserting data. Then the binary tree needs to re-balanced itself again which is costly. Because now there will be two operations, one is manipulating the table and another one is rebalancing the tree for indexing. So, it is expensive. That is why using excessive index is harmful.

- **What types of indexes do you know?**
  - Unique index - does not allow duplicate values in a table column. It helps data integrity.
  - Clustered index - defines the physical order of records of a table and performs data searching based on the key values. A table can have only one clustered index.
  - Non-clustered index - This index order is different from the actual physical order of the data of the table. That means actual data is stored in one place and non-clustered-index is stored in another place. A table can have multiple non-clustered index.

- **What is a schema?**
  - A collection of database structural elements, like - tables, store procedures, functions, indexes and triggers.

- **What is SQL comment?**
  - As like any other language, it is the statement which is gonna ignored by SQL engine.
  
- **What is a NULL value? How is it different from zero or a blank space?**
  - `NULL` means the absence of the data in a particular column. But zero is a valid numeric number and blank space is a zero-length valid string. 
  
- **SQL vs NoSQL**
  - SQL database is structured, relational with predefined schemas. But NoSQL is non-relational, schema-less which is designed to handle unstructured or semi-structured data.
  
- **What are some common challenges when working with SQL databases?**
  - performance tuning for large datasets
  - managing indexing strategies
  - data integrity with constraints
  - handling concurrent transactions
  - optimizing query execution

- **What is a function in SQL?**
  - A database object representing a set of sql statements frequently used for a certain task. Given some input, it performs some operation, may change data and give the result. There are two types of functions.
    - Aggregate functions: work on multiple rows and return a single result, like - AVG, SUM, MIN, MAX etc
    - Scalar functions: Work on single input and return a single result, like - LEN(), NOW(), UCASE() etc.

- **What is the difference between local and global variables?**
  - Local variable: It is only accessible inside a function in which they are declared.
  - Global variable: It is declared outside any function, stored in fixed memory structure which can be used throughout the entire program.

- **What is the difference between LEFT JOIN and LEFT OUTER JOIN?**
  - Absolutely no difference. `OUTER` keyword is optional.

- **What is a stored procedure, and how is it different from a function?**
  - Store procedure can be executed as a single unit of task, like - inserting, updating or deleting. It may or may not return values (single or multiple). It also supports transactions. It cannot be called from `SELECT` statement. But in function, we will compute data and return single value, that's it. It should not modify any data (should not have any side-effects) or do any transaction related work. A function can be called from `SELECT` statement. 

- **What set operators do you know?**
  - UNION – returns the records by at least one of two queries (excluding duplicates)
  - UNION ALL – returns the records obtained by at least one of two queries (including duplicates)
  - INTERSECT – returns the records obtained by both queries
  - EXCEPT (called MINUS in MySQL and Oracle) – returns only the records obtained by the first query but not the second one

- **What is a composite primary key?**
  - A primary key made of multiple columns.

- **In which order does the interpreter execute the common statements in the SELECT query?**
  - FROM - ON - WHERE - GROUP BY - HAVING - SELECT (this is interesting!) - DISTINCT - ORDER BY - LIMIT/OFFSET.

- **What is a view, and why use it?**
  - View is a virtual table containing a subset of data retrieved from multiple tables (or views). It takes very little space, simplify complex queries, summarizing data from multiple tables. 

- **Can we create a view based on another view?**
  - Yes, it is possible and called as nested-views. But we should avoid nesting multiple views since the code becomes difficult to read and debug.

- **Can we still use a view if the original table is deleted?**
  - Actually we cannot delete the table because the view is dependent on it. So, at first we need to drop the table and then drop the view.

- **What are the possible values of a BOOLEAN data field?**
  - In postgresql, `TRUE`, `FALSE` and `NULL`. But for microsoft SQL server, bit datatype is used as integers, like 1(true) or 0 (false).

- **What is normalization in SQL, and why use it?**
  - It is a process of database design that includes organising and restructuring data to reduce data redundancy, dependency, duplication and inconsistency. It helps to enhance data integrity, more efficient data access and security control and greater query flexibility.

- **What is denormalization in SQL, and why use it?**
  - It is the opposite of normalisation and introduces data redundancy and combines data from multiple tables. It optimizes the performance of the database infrastructure in situations where read operations are more important than write operations as it helps avoid complex joins and reduces the time of query running.

- **What is the difference between nested and correlated subqueries?**
  - correlated subquery - it is an inner query nested in a bigger query (outer) that has values from the outer query for execution. That means this subquery depends on outer query. 
  - non-correlated subquery - it is subquery that does not depend on outer query. It is independent.

- **What is the difference between the DELETE and TRUNCATE statements?**
  - DELETE - DML operation. It can be rolled back. And we can delete one or more rows by where operation. It is slower as it performs this action row-by-row. We can still perform this if `foreign key` exits. It does not reset the identity. We need to manually do this. It does the row-level-lock. Trigger is fired for delete.
  - TRUNCATE - DDL operation. It is non-reversible if it is not inside a transaction. It is faster as it does not go row-by-row. We cannot perform this operation if the table contains `foreign key`. It resets the identity to the initial value. It does the table-level-lock. Trigger is not fired for this action.

- **What is lock? What kind of locks are present**
  - 
  - Shared lock - 
  - Exclusive lock - 

- **What is 1NF, 2NF, 3NF?**
  - 1NF: 
    - a single cell must not hold more than one value, like course column - C, Java, Python. It must have 3 different rows for each course.
    - No duplicate rows or columns
  - 2NF:
    - must be 1NF
    - No partial dependency. All non-key attributes are fully dependent on a primary key
  - 3NF:
    - must be 2 NF  
    - have no transitive partial dependency
  
  - Source - [Freecodecamp](https://www.freecodecamp.org/news/database-normalization-1nf-2nf-3nf-table-examples)
- **What is database cursor?**

- **What is materialised view? Why it is different from Views**
  - Materialised view is kind of view where data is already fetched from multiple tables and served when needed immediately. But traditional view is just an object with defined query. So, when the view is needed, the query is executed every time and data is returned. So, it is expensive but fetched data is always up-to-date. On the other hand, in materialised view, data fetching is faster as data is fetched previously and cached like a table. So, no need to run the underlying query again and again. But the problem is data may not be up-to-date. So, we need to configure how we are gonna refresh our materialised view with schedule or some other technique.
  - Source - [AWS](https://aws.amazon.com/what-is/materialized-view/)

- **Partitioning vs Sharding**

- **What is transaction? please describe ACID properties**
  - Transaction is a sequence of operations performed as a single logical unit of work. These operations may involve reading, writing, updating or deleting data in database. It will be complete only if all its operations are successfully executed, otherwise the transaction will be rolled back, ensuring data consistency in the database. 
  - These are the principles of database transactions. 
    - Atomicity - All the statements of a single transaction must pass or fail together. We can think this as like `atom`, if success, then success, if fail then fail. No middle dangling statements.
    - Consistency - Data must be consistent throughout the database after transaction. If there is a transfer happened to one column to another column, then both plus and minus must be happened in two columns.
    - Isolation - Each transaction is separate from another transaction. So, if anything happened in one transaction, that calculation must be no effect to another transaction. Well, there are some `Isolation level` for this criteria. We can tune this level as per our need.
    - Durability - Transaction must be persisted. If the database crashes or powered off suddenly, when it comes back, our committed data must present in the database.
  
  - Source - [MongoDB](https://www.mongodb.com/resources/basics/databases/acid-transactions)

- **What is Isolation level?**
  - It is a property set for a transaction. By setting this, we can configure how far we want to go with our transaction data effected by other transaction. It is a trade-off between speed and accurate data. In a concurrent transactional environment, for the lowest level of isolation level, we will get faster data but it may occur inaccurate data. On the other hand, for the highest level, we are ensuring top-notch accurate data but that will not give any concurrent environment to us but a serialised thing, where we will get slower response. Because everything get locked to ensure the perfect data accuracy. Here are the four levels.
    - Read uncommitted - Lowest level of isolation. By this, one transaction can read other transaction's data where that is not committed yet. So, it is the fastest in concurrent environment. How funny! Most of the database, like - Postgres does not support this level at all. We should only use this level if we are 100% sure that when we are reading data inside a transaction, it will be never changed by any means. `Dirty read` is possible here.
    - Read committed - It is weakest level of isolation implemented by most of the databases. And it is the default in Postgres. The concept is - our transaction can see the `committed data`from other transaction. But it has minor inconsistencies, like `non-repeatable read` and `phantom`. If we re-read a row which is updated in no time which is just committed in another transaction, then we can see the new value for that row. 
    - Repeatable read - It is intermediate level of isolation. It ensures that inside a transaction, if we re-read any row twice, it will give the same value whatever the row is changed and committed in another transaction, it does not matter. So, it prevents the `non-repeatable read` anomaly but maybe still `phantom` anomaly can occur. Let's say we are calculating user's total balance. This level ensures that balance does not change in the time calculation. It is ideal solution for read-only transactions. For read-write transactions, `serializable` or `read-committed` is better choice.
    - Serializable - It is the highest level of isolation. So, it is the safest and slowest level. Transactions are completely isolated from each other. It is executed as if there is only one transaction in the system. It prevents `dirty reads`, `non-repeatable reads`, `phantom reads`. It guarantees that each transaction sees the consistent view of database even there are concurrent transactions. It is the best option for banking or financial payments that transfers money from one account to another one.
  -Source - [Cockroach labs](https://www.cockroachlabs.com/blog/sql-isolation-levels-explained/), [Microsoft](https://learn.microsoft.com/en-us/sql/t-sql/statements/set-transaction-isolation-level-transact-sql?view=sql-server-ver17)

- **What is dirty read, non-repeatable read and phantom read?**
  - Dirty read - When we can read data from other transaction which is not committed yet. 
  - Non-repeatable read - If we re-read a same row value (which is committed in another transaction) inside a transaction, we may get different result. It won't happen in `repeatable-read` and `serializable` isolation levels.
  - phantom read - It is kind of like non-repeatable read with a slight difference. Like - we will re-run the query but we will get new result set, like - newly inserted row will happen or maybe any row get deleted (this insert or delete is already committed in another transaction). But it won't happen in `serializable` isolation level.

- **How database handles isolation?**

- **What is Transaction?**
