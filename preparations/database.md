## Contents

* [Basic Questions](#basic-questions)
* [Question Collection](#question-collection)

### Basic Questions

### Question Collection

##### MySQL

* <b>Define SQL</b></br>
 SQL stands for Structured Query Language. SQL is a programming Language designed specially for managing data in Relational Database Management System (RDBMS).

* About MySQL

MySQL is an open-source relational database management system (RDBMS). The name is derived from a combination of “My” which stands for the name of the daughter of the co-founder Michael Widenius, and “SQL” which is stands for Structured Query Language.

MySQL is owned by Oracle, though initially owned and sponsored by a single for-profit firm, the Swedish company MYSQLAB. The MYSQL development project makes its source code accessible under the GNU General Public License terms, including a range of propriety agreements. You can get various paid editions with additional functionality for propriety use.

* <b>What is MySQL?</b></br>

MySQL is a multithreaded, multi-user SQL database management system which has more than 11 million installations. This is the world's second most popular and widely used open source database. It is interesting how MySQL name was given to this query language. The term My is coined by the name of the daughter of co-founder Michael Widenius's daughter, and SQL is the short form of Structured Query Language. Using MySQL is free of cost for the developer, but enterprises have to pay a license fee to Oracle.

Formerly MySQL was initially owned by a for-profit firm MySQL AB, then Sun Microsystems bought it and then Oracle bought Sun Microsystems, so Oracle currently owns MySQL.

MySQL is an Oracle-supported Relational Database Management System (RDBMS) which is based on structured query language. MySQL supports wide ranges of operating systems most famous of those include Windows, Linux & UNIX. Although it is possible to develop a wide range of application with MySQL, it is only used for web applications & online publishing. It is a fundamental part of an open source enterprise known as Lamp.

<b>What is Lamp?</b>

Lamp is a platform used for web development. Lamp uses Linux, Apache, MySQL, and PHP as an operating system, web server, database & object-oriented scripting language respectively. And hence abbreviated as LAMP.

* <b>In which language MySQL has been written?</b></br>
MySQL is written in C and C++, and its SQL parser is written in yacc.

* <b>What are the technical specifications of MySQL?</b></br>
MySQL has the following technical specifications -

 * Flexible structure
 * High performance
 * Manageable and easy to use
 * Replication and high availability
 * Security and storage management
 * Drivers
 * Graphical Tools
 * MySQL Enterprise Monitor
 * MySQL Enterprise Security
 * JSON Support
 * Replication & High-Availability
 * Manageability and Ease of Use
 * OLTP and Transactions
 * Geo-Spatial Support

* <b>What are the technical features of MySQL? </b></br>
MySQL database software is a client or server system which includes

 * Multithreaded SQL server supporting various client programs and libraries
 * Different backend
 * Wide range of application programming interfaces and
 * Administrative tools.


*  <b>What is RDBMS? Explain its features?</b></br>
A Relational Database Management System (RDBMS) is the most widely used database Management System based on the Relational Database model.</br>
Features of RDBMS:
 * Stores data in tables.
 * Tables have rows and column.
 * Creation and Retrieval of Table is allowed through SQL.

* <b>What is the difference between MySQL and SQL?</b></br>
SQL is known as the standard query language. It is used to interact with the database like MySQL. MySQL is a database that stores various types of data and keeps it safe.

A PHP script is required to store and retrieve the values inside the database.

SQL is a computer language, whereas MySQL is a software or an application

SQL is used for the creation of database management systems whereas MySQL is used to enable data handling, storing, deleting and modifying data

* <b>Why do we use the MySQL database server?</b></br>
First of all MYSQL server is free to use for developers and a small fee for enterprises.

MySQL server is open source.

The community of MySQL is tremendous and supportive hence any help regarding MySQL is resolved as soon as possible.

MySQL has very stable versions available, as MySQL has been in the market since a long time so all bugs arising in the previous builds have been continuously removed and a very stable version is provided after every update.

The MySQL database server is very fast, reliable and easy to use. You can easily use and modify the software. MySQL software can be downloaded free of cost from the internet.

* <b></b></br>
* <b>What is Data Mining?</b></br>
  Data Mining is a subcategory of Computer Science which aims at extraction of information from set of data and transform it into Human Readable structure, to be used later.

*  <b>What is an ERD?</b></br>
 ERD stands for Entity Relationship Diagram. Entity Relationship Diagram is the graphical representation of tables, with the relationship between them.

* <b>What is the difference between Primary Key and Unique Key?</b></br>
 Both Primary and Unique Key is implemented for Uniqueness of the column. Primary Key creates a clustered index of column where as an Unique creates unclustered index of column. Moreover, Primary Key doesn’t allow NULL value, however Unique Key does allows one NULL value.

* <b> How to store picture file in the database. What Object type is used?</b></br>
 Storing Pictures in a database is a bad idea. To store picture in a database Object Type ‘Blob’ is recommended.

* <b>What is Data Warehousing?</b></br>
A Data Warehousing generally refereed as Enterprise Data Warehousing is a central Data repository, created using different Data Sources.

* <b>What are indexes in a Database. What are the types of indexes?</b></br>
Indexes are the quick references for fast data retrieval of data from a database. There are two different kinds of indexes.

 <b>Clustered Index:</b>
 * Only one per table.
 * Faster to read than non clustered as data is physically stored in index order.</br>

 <b>Non­clustered Index:</b>
 * Can be used many times per table.
 * Quicker for insert and update operations than a clustered index.


* <b>What is a Trigger? How many TRIGGERS are possible in MySQL?</b></br>
A trigger is a set of codes that executes in response to some events.
There are only six triggers are allowed to use in MySQL database and they are.

 * Before Insert
 * After Insert
 * Before Update
 * After Update
 * Before Delete
 * After Delete

* <b>What is Heap table?</b></br>

 - HEAP tables are found in memory.
 - They are used for high speed storage on temporary basis.

 Some of their characteristics are:
 - They do not allow BLOB or TEXT fields.
 - Only comparison operators like =, <, >, = >, =< can be used with them.
 - AUTO_INCREMENT is not supported by HEAP tables
 - Indexes should be NOT NULL

* <b>How do you control the max size of a HEAP table?</b></br>
Maximum size of Heap table can be controlled using MySQL config variable called `max_heap_table_size`.

* <b>What are the advantages of MySQL in comparison to Oracle?</b></br>
 - MySQL is a free, fast, reliable, open source relational database while Oracle is expensive, although they have provided Oracle free edition to attract MySQL users.
 - It is portable.
 - GUI with command prompt.
 - Administration is supported by MySQL Query Browser.
 - MySQL uses only just under 1 MB of RAM on your laptop while Oracle 9i installation uses 128 MB.
 - MySQL is great for database enabled websites while Oracle is made for enterprises.

* <b>What are the disadvantages of MySQL?</b></br>

 * MySQL is not so efficient for large scale databases.
 * It does not support COMMIT and STORED PROCEDURES functions version less than 5.0.
 * Transactions are not handled very efficiently.
 * Functionality of MySQL is highly dependent of other addons.
 * Development is not community driven.

* <b>Give string types available for column?</b></br>
The string types are:

 * SET
 * BLOB
 * ENUM
 * CHAR
 * TEXT
 * VARCHAR

* <b>How to get current MySQL version?</b></br>
`SELECT VERSION ();` is used to get the current version of MySQL.

* <b>What storage engines are used in MySQL? </b></br>
Storage engines are called table types and data is stored in files using various techniques.

Technique involves:

 * Storage mechanism
 * Locking levels
 * Indexing
 * Capabilities and functions.


* <b>Differentiate between FLOAT, DOUBLE and REAL.</b></br>
FLOAT stores floating point numbers with accuracy up to eight places and has four bytes while DOUBLE stores floating point numbers with accuracy upto 18 places and has eight bytes. REAL is a synonym of FLOAT for now.


* <b>How would you select all the users, whose phone number is null</b></br>
 `Select user_name FROM users WHERE ISNULL(user_phonenumber)`.

* <b>What does myisamchk do?</b></br>
It compresses the MyISAM tables, which reduces their disk or memory usage.

* <b>What is the difference between MyISAM Static and MyISAM Dynamic?</b></br>
In MyISAM static all the fields will have fixed width. The Dynamic MyISAM table will have fields like TEXT, BLOB, etc. to accommodate the data types with various lengths.

MyISAM Static would be easier to restore in case of corruption.

* <b>How is MyISAM table stored?</b></br>
MyISAM table is stored on disk in three formats.
 - ‘.frm’ file – storing the table definition
 - ‘.MYD’ (MYData) - data file
 - ‘.MYI’ (MYIndex) – index file

* <b>Explain advantages of MyISAM over InnoDB?</b></br>
 - MyISAM follows a much more conservative approach to disk space management.
 - Storing each MyISAM table in a separate file, which can be further compresses, if required.
 - InnoDB stores the tables in tablespace. Further optimization is difficult with them.


* <b>How can we convert between Unix & MySQL timestamps?</b></br>
 - MySQL timestamp can be converted into Unix timestamp using the command UNIX_TIMESTAMP.
 - Unix timestamp can be converted into MySQL timestamp using the command FROM_UNIXTIME.

* <b>What, if a table has one column defined as TIMESTAMP?</b></br>
Timestamp field gets the current timestamp whenever the row gets altered.

* <b>What happens when the column is set to AUTO INCREMENT and if you reach maximum value in the table?</b></br>
It stops incrementing. Any further inserts are going to produce an error, since the key has been used already.

* <b>How can we find out which auto increment was assigned on Last insert?</b></br>
LAST_INSERT_ID will return the last value assigned by Auto_increment and it is not required to specify the table name.

* <b>How can you see all indexes defined for a table?</b></br>
Indexes are defined for the table by:

`SHOW INDEX FROM <tablename>;`

* <b>What is BLOB?</b></br>

 - BLOB stands for binary large object.
 - It that can hold a variable amount of data.

There are four types of BLOB based on the maximum length of values they can hold:

 - TINYBLOB
 - BLOB
 - MEDIUMBLOB
 - LONGBLOB

* <b>What is TEXT(Non-Standard string types)?</b></br>
TEXT is case-insensitive BLOB. The four types of TEXT are:

 - TINYTEXT
 - TEXT
 - MEDIUMTEXT
 - LONGTEXT

* <b>What is the difference between BLOB and TEXT?</b></br>
 - In BLOB sorting and comparison is performed in case-sensitive for BLOB values.
 - In TEXT types sorting and comparison is performed case-insensitive.

* <b>How would you enter Characters as HEX Numbers?</b></br>
 - To enter characters as HEX numbers, you can enter HEX numbers with single quotes and a prefix of (X).
 - Alternatively, just prefix HEX numbers with (Ox).

* <b>How will you export tables as an XML file in MySQL?</b></br>
MYSQL’s query browser has a provision called “Export Result Set” which allows the tables to be exported as XML.

* <b>What is the use of `i-am-a-dummy` flag in MySQL?</b></br>
Using the i-am-dummy flag makes the SQL engine refuse any Updates or deletes to execute if the WHERE clause is not present. It is very useful when using delete statements. Using i-am-dummy flag will not allow the following statement to execute:
 `Delete from employee;`

* <b>What are the differences between MySQL_fetch_array(), MySQL_fetch_object(), MySQL_fetch_row()?</b></br>

Mysql_fetch_object returns the result from the database as objects while mysql_fetch_array returns result as an array. This will allow access to the data by the field names.

E.g. using mysql_fetch_object field can be accessed as $result->name and using mysql_fetch_array field can be accessed as $result->[name]. mysql_fetch_row($result):- where $result is the result resource returned from a successful query executed using the mysql_query() function.

  ```sql
  $result = mysql_query("SELECT * from students");
  while($row = mysql_fetch_row($result))
  {
        Some statement;
  }
   ```
* <b>What is difference between mysql_connect and mysql_pconnect?</b></br>
Mysql_connect() opens a new connection to the database while mysql_pconnect() opens a persistent connection to the database. This means that each time the page is loaded mysql_pconnect() does not open the database. Mysql_close() cannot be used to close the persistent connection. Though it can be used to close mysql_connect().

 Mysql_connect:

 - Opens a new connection to the database.
 - The database connection can be closed.
 - Opens the page every time the page is loaded.

 Mysql_pconnect:

 - Opens a persistent connection to the database.
 - The database connection can not be closed.
 - The page need not be opened every time the page is loaded.

* <b>What is MySQL data directory? How to determine the location of the data directory?</b></br>
MySQL stores its data on the disk on the data dictionary. Each subdirectory under this data dictionary represents a MySQL database, inside those directories. By default the information managed my MySQL = server mysqld is stored in data directory.A default location of data directory in windows is `C:\mysql\data or C:\Program Files\MySQL\MySQL Server 5.0 \data.`

* <b>What you can use Regular Expression for in MySQL? Support your answer with an example.</b></br>

 Regular expressions in MySql are used in queries for searching a pattern in a string.

 * \* Matches 0 more instances of the string preceding it.
 * \+ matches 1 more instances of the string preceding it.
 * \? Matches 0 or 1instances of the string preceding it.
 * \. Matches a single character.
 * [abc] matches a or b or z
 * | separates strings
 * ^ anchors the match from the start.

 REGEXP can be used to match the input characters with the database.

 Example:

 The following statement retrieves all rows where column employee_name contains the text 1000 (example salary):
 ```sql
Select employee_name
From employee
Where employee_name REGEXP ‘1000’
Order by employee_name
```
 “.” Can be used to match any single character. “|” can be used to match either of the two strings

* <b>What are the applications required to support MYSQL?</b></br>
The applications that are required to support MySQL are as follows:

1. php-mysql MySQL database is used specifically to support PHP
2. perl-DBI : provides generic Perl interface for interacting with relational databases
3. perl-DBD-MySQL database specific support for Perl
4. Web server is required to configure the database and its configuration
5. Programming language is required which supports MySQL.

* <b>Write a command with which MySQL table can be repaired</b></br>
 The command syntax with which mysql table can be repaired is as follows:
 ```sql
REPAIR TABLE tablename;
REPAIR TABLE tablename QUICK;
REPAIR TABLE tablename EXTENDED;
```
The command will just do as it says repair a specified table, but if QUICK or EXTENDED is used then the meaning of it changes. In case of QUICK it will repair only the index tree, whereas in case of EXTENDED it will create index row by row and repair it.

* <b>What are the different tables present in MySQL?</b></br>
There are many tables that remain present by default. But, MyISAM is the default database engine used in MySQL. There are five types of tables that are present:

1. MyISAM
2. Heap
3. Merge
4. INNO DB
5. ISAM


* <b>What does the file with the extension: frm, myd, and myi contain?</b></br>

MySQL default table type is MyISAM, where there are three kind of files that are stored inside MyISAM. The file names begin with the table name and have the extensions such as frm, myd and myi. The explanation of each file is given below:

.frm file consists of the table definition that are stored in the database
.myd is an extension that is used by a data file.
.myi is an extension that is used by index file.

* <b>What is the difference between MYSQL and SQL?</b></br>
- SQL is known as standard query language, as the name implies it is the language which is used to interact with the database like MySQL.

- MySQL is a database that store various types of data and keep it safe. A PHP script is required to store and retrieve the values inside the database.

* <b>How database are managed?</b></br>
Database is a collection of data and it is managed by a database server, which is a special program that is also known as MySQL database server. Application that you create usually communicates with the database server in the language which it can understand; mostly SQL language is used for communication. Database server in return interacts with the web server on same server or computer. Database server and web server result in the data which is being shown on the web.

* <b>Why phpMyAdmin is used for MYSQL?</b></br>
PhpMyAdmin is a very popular and easy to use GUI tool that can allow SQL commands to be run to create database, create tables, insert data and retrieve it. It provides a web based interface to the user for the ease of use. phpMyAdmin allows user to manage everything from one place and no other installation is required in the computer after this.

* <b>What is the difference between a database and a table?</b></br>
There is a major difference between a database and a table. The differences are as follows:

1. Tables are a way to represent the division of data in a database. Whereas, database is a collection of tables and data.
2. Tables group the data in relation with each other and create a dataset; this dataset will be used in the database. The data which are stored in the table in any form is a part of the database, but opposite is not true.

* <b>What is the difference between truncate and delete?</b></br>
D
elete command is used to delete data from a table for example Remove emails where we write a script to delete the customer’s data. It deletes the rows of data from a table. The syntax of it as follows:
`DELETE FROM table_name`

Whereas, truncate is very dangerous command and should be used carefully as it deletes every row from a table. The syntax of it as follows:
`TRUNCATE TABLE "table_name"`

* <b>How do you display the structure of the table</b></br>
 `Describe table_name`

* <b>How important is to list the column names when doing an INSERT?</b></br>
It is not important to list the column names when doing using an INSERT command as you can provide the column information and values in the table in the same order in which they appear in the table structure. It is safer and convenient way to specify the column names as it will keep the count of the column you are visiting.

* <b>Where’s database data actually stored? Is there a way to see the files which are stored?</b></br>

Database data is usually get stored in the computer hard-disk and you can manage the data by the database program like MySQL and phpAdmin. The files can be seen but database files remain in binary format so it can be opened and read but, you have to put extra effort to understand it. SQL is given for the purpose of interacting with the database and read the database and retrieve the information out of it.

* <b>Why to use CHAR instead of VARCHAR in the database?</b></br>
CHAR is much more accurate and efficient to use. CHAR doesn’t have to keep a count of the variable length. It is more efficient when you have to use it for a text column which is of an exact length. Char is used for the data which are fixed, but VARCHAR is used for data like password, which are variable.

* <b>Differentiate CHAR_LENGTH and LENGTH?</b></br>
CHAR_LENGTH  is character count whereas the LENGTH is byte count. The numbers are same for Latin characters but they are different for Unicode and other encodings.

* <b>How to represent ENUMs and SETs internally? </b></br>
ENUMs and SETs are used to represent powers of two because of storage optimizations.

* <b>What is the difference between CHAR and VARCHAR?</b></br>
A list of differences between CHAR and VARCHAR:

 * CHAR is variable-length whereas VARCHAR is of fixed length.
 * CHAR and VARCHAR types are different in storage and retrieval.
 * CHAR column length is fixed to the length that is declared while creating a table. The length value ranges from 1 and 255.
 * When CHAR values are stored when they are right-padded using spaces to a specific length. Trailing spaces are removed when CHAR values are retrieved.
 * CHAR uses static memory allocation whereas VARCHAR uses dynamic memory allocation.
 * CHAR is 50% faster than VARCHAR.
 * The maximum no. of character CHAR data type can hold is 255 character while VARCHAR can hold up to 4000 character


* <b>What are ENUMs used for in MySQL?</b></br>
ENUM is used to limit the possible values and store it together. It is a function that can be created to store the similar values together. It is used in creation of table.

The syntax of it is as follows:
```sql
CREATE TABLE months (month ENUM “January”, “February”, “March”,…);
INSERT months VALUES (“April”);
```

* <b>What is the usage of ENUMs in MySQL?</b></br>
ENUM is a string object used to specify set of predefined values and that can be used during table creation.

 ```SQL
 Create table size(name ENUM('Small', 'Medium', 'Large'));
 ```

* <b>What is the purpose of -> in the MySQL terminal?</b></br>
-> prompt in the command of MySQL indicates that a single statement is being entered across multiple lines. From this prompt MySQL interprets that you haven’t finished entering the statements. It has no impact of enter which you might press to go to the next line. MySQL will execute the statement only when you will insert the semicolon in the end which it recognizes.

* <b>How to find the unique values if the value in the column is repeated?</b></br>
If the values in the column of a table are repeating and a unique value has to be found then the following command can be used in the query:
`SELECT DISTINCT user_firstname FROM users;`

There is another command which can be used to find the command to see the distinct values as:
`SELECT COUNT (DISTINCT user_firstname) FROM users;`

* <b>What is the difference between Unix timestamps and MySQL timestamps?</b></br>
The unix timestamp is stored as 32 bit integer whereas, MySQL timestamps are stored in 32 bit integers but represented differently then UNIX timestamps like YYYY-MM-DD HH:MM:SS format. Unix timestamp is given as month-day-year-HH:MM:SS..

* <b>What does a TIMESTAMP do on UPDATE CURRENT_TIMESTAMP data type?</b></br>
TIMESTAMP column is updated with Zero when the table is created.  UPDATE CURRENT_TIMESTAMP modifier updates the timestamp field to  current time whenever there is a change in other fields of the table.


* <b>How would you check if MySql service is running or not?</b></br>
 Issue the command “service mysql status” in ‘Debian’ and “service mysqld status” in RedHat. Check the output, and all done.

* <b>If the service is running/stop how would you stop/start the service?</b></br>
 To start MySql service use command as service mysqld start and to stop use service mysqld stop.

* <b>How will you switch to a database, and start working on that?</b></br>
To use or switch to a specific database run the command on mysql shell as: `use database_name;`

* <b> How will you get the Field Name and Type of a MySql table?</b></br>
To get the Field Name and Type of a table use the command on mysql shell as: `describe table_name;`

* <b>What is the difference between heap table and temporary table?</b></br>
<b>Heap tables:</b>

Heap tables are found in memory. They are used for high-speed storage on a temporary basis. They do not allow BLOB or TEXT fields.

Heap tables do not support AUTO_INCREMENT.

Indexes should be NOT NULL.

<b>Temporary tables:</b>

The temporary tables are used to keep the transient data. Sometimes it is beneficial in cases to hold temporary data. The Temporary table is deleted after the current client session terminates.

<b>Main differences:</b>

The heap tables are shared among clients while temporary tables are not shared.

Heap tables are just another storage engine, while for temporary tables you need a special privilege (create temporary table).

* <b>How to get the current date in MySQL?</b></br>
To get current date, use the following syntax:

`SELECT CURRENT_DATE();`  

* <b>What are the security alerts while using MySQL?</b></br>
 * Install antivirus and configure the operating system's firewall.
 * Never use the MySQL Server as the UNIX root user.
 * Change root username and password Restrict or disable remote access.

* <b>How to display Nth highest salary from a table in a MySQL query?</b></br>
Let us take a table named the employee.
To find Nth highest salary is:
`select distinct(salary)from employee order by salary desc limit n-1,1`
if you want to find 3rd largest salary:

`select distinct(salary)from employee order by salary desc limit 2,1`

* <b>What is MySQL default port number?</b></br>
MySQL default port number is 3306.

* <b>What is REGEXP?</b></br>
REGEXP is a pattern match using a regular expression. A Regular expression is a powerful way of specifying a pattern for a sophisticated search.

Basically it is a special text string for describing a search pattern. To understand it better you can think of a situation of daily life when you search for .txt files to list all text files in the file manager. The regex equivalent for .txt will be .\*\.txt.

* <b>How many columns can you create for an index?</b></br>
You can create maximum of 16 indexed columns for a standard table.

* <b>What is the difference between NOW() and CURRENT_DATE()?</b></br>
NOW() command is used to show current year, month, date with hours, minutes and seconds while CURRENT_DATE() shows the current year with month and date only.

* <b>How do you get the month from a timestamp</b></br>
 `Select month(january_timestamp) from tablename`

* <b>What is the query to display top 20 rows?</b></br>
SELECT * FROM table_name LIMIT 0,20;

* <b>What is save point in MySQL?</b></br>
A defined point in any transaction is known as savepoint.

SAVEPOINT is a statement in MySQL which is used to set a named transaction save point with a name of identifier.

* <b>What is SQLyog?</b></br>
SQLyog program is the most popular GUI tool for admin. It is the most popular MySQL manager and admin tool. It combines the features of MySQL administrator, phpMyadmin and others MySQL front ends and MySQL GUI tools.

* <b>What are the different column comparison operators in MySQL?</b></br>
The =, <>, <=, <, >=, >, <<, >>, < = >, AND, OR or LIKE operator are the comparison operators in MySQL. These operators are generally used with SELECT statement.

* <b>Write a query to count the number of rows of a table in MySQL.</b></br>
SELECT COUNT user_id FROM users;

* <b>Write a query to retrieve a hundred books starting from 20th.</b></br>
SELECT book_title FROM books LIMIT 20, 100;

* <b>Write a query to select all teams that won either 1, 3, 5 or 7 games.</b></br>
SELECT team_name FROM team WHERE team_won IN (1, 3, 5, 7);

* <b>What are the advantages of MyISAM over InnoDB?</b></br>
MyISAM follows a conservative approach to disk space management and stores each MyISAM table in a separate file, which can be further compresses, if required. On the other hand, InnoDB stores the tables in tablespace. Its further optimization is difficult.

* <b>What is the use of mysql_close()?</b></br>
Mysql_close() cannot be used to close the persistent connection. Though it can be used to close connection opened by mysql_connect().

* <b>Explain Access Control Lists.</b></br>
An ACL is a list of permissions which are associated with an object. This list is the basis for MySQL server’s security model and it helps in troubleshooting problems like users not being able to connect. MySQL keeps the Access Control Lists cached in memory and whenever the user tries to authenticate or execute a command, MySQL checks the permission required for the object and if the permissions are available then execution completes successfully.

* <b>What is InnoDB?</b></br>
InnoDB is a storage database for SQL. The ACID-transactions are also provided in addition InnoDB also includes support for the foreign key. Initially owned by InnobaseOY now belongs to Oracle Corporation after it acquired the latter since 2005.

* <b>How would you change a table to InnoDB</b></br>
 `ALTER TABLE name_file ENGINE innodb`

* <b>What is ISAM?</b></br>
It is a system for file management developed by IBM which allows records to access sequentially or even randomly.

* <b>How can we run batch mode in MySQL?</b></br>
To perform batch mode in MySQL we use the following command:

mysql;

mysql mysql.out;

* <b>What are federated tables?</b></br>
Federated tables are tables which points to the tables located on other databases on some other server.

* <b>What is the difference between primary key and candidate key?</b></br>
To identify each row of a table, a primary key is used. For a table, there exists only one primary key.

A candidate key is a column or a set of columns which can be used to uniquely identify any record in the database without having to reference any other data.

* <b>How MySQL Optimizes DISTINCT?</b></br>
DISTINCT is converted to a GROUP BY on all columns and it will be combined with ORDER BY clause.
`SELECT DISTINCT t1.a FROM t1,t2 where t1.a=t2.a;`
* <b>What are the drivers in MySQL?</b></br>
Following are the drivers available in MySQL:

 * PHP Driver
 * JDBC Driver
 * ODBC Driver
 * C WRAPPER
 * PYTHON Driver
 * PERL Driver
 * RUBY Driver
 * CAP11PHP Driver
 * Ado.net5.mxz

* <b>What Is DDL, DML, And DCL?</b></br>
Majorly SQL commands can be divided into three categories i.e. DDL, DML & DCL. Data Definition Language (DDL) deals with all the database schemas, and it defines how the data should reside in the database. Commands like Create TABLE and ALTER TABLE are part of DDL.

Data Manipulative Language (DML) deals with operations and manipulations on the data the commands in DML are Insert, Select etc.

Data Control Languages (DCL) are related to the Grant and permissions. In short, the authorization to access any part of database is defined by these.

* <b>What do you mean by % and _ in the LIKE statement?</b></br>
% corresponds to 0 or more characters, _ is exactly one character in the LIKE statement.

* <b>What is the LIKE?</b></br>
 A LIKE pattern match, which succeeds only if the pattern matches the entire value.

* <b>How can we get the number of rows affected by query?</b></br>
Number of rows can be obtained by `SELECT COUNT (user_id) FROM users;`

* <b> Is Mysql query is case sensitive?</b></br>
 No.
 ```SQL
 SELECT VERSION(), CURRENT_DATE;
SeLect version(), current_date;
seleCt vErSiOn(), current_DATE;
 ```
 All these examples are same. It is not case sensitive.

* <b>What is the difference between the LIKE and REGEXP operators?  </b></br>
 LIKE and REGEXP operators are used to express with ^ and %.
 ```SQL
 SELECT * FROM employee WHERE emp_name REGEXP "^b";
SELECT * FROM employee WHERE emp_name LIKE "%b";
 ```

* <b>How can we run batch mode in mysql?</b></br>
Following commands are used to run in batch mode: </br>
```SQL
mysql ;
mysql mysql.out
```

* <b>How do you concatenate strings in MySQL</b></br>
 `CONCAT (string1, string2, string3)`

* <b>What are all the Common SQL Function?</b></br>

 * CONCAT(A, B) – Concatenates two string values to create a single string output. Often used to combine two or more fields into one single field.

 * FORMAT(X, D) – Formats the number X to D significant digits.

 * CURRDATE(), CURRTIME() – Returns the current date or time.

 * NOW() – Returns the current date and time as one value.

 * MONTH(), DAY(), YEAR(), WEEK(), WEEKDAY() – Extracts the given data from a date value.

 * HOUR(), MINUTE(), SECOND() – Extracts the given data from a time value.

 * DATEDIFF(A, B) – Determines the difference between two dates and it is commonly used to calculate age

 * SUBTIMES(A, B) – Determines the difference between two times.

 * FROMDAYS(INT) – Converts an integer number of days into a date value.
* <b></b></br>
</br><b>Read more</b>:
* [10 MySQL Database Interview Questions for Beginners and Intermediates](http://www.tecmint.com/10-mysql-database-interview-questions-for-beginners-and-intermediates/)
* [100 MySQL interview questions](http://www.careerride.com/MySQL-Interview-Questions.aspx)
* [15 Basic MySQL Interview Questions for Database Administrators](http://www.tecmint.com/basic-mysql-interview-questions-for-database-administrators/)
* [28 MySQL interview questions from JavaTPoint.com](http://www.javatpoint.com/mysql-interview-questions)
* [40 Basic MySQL Interview Questions with Answers](http://www.testingbrain.com/interview/mysql-interview-questions.html)
* [Top 50 MySQL Interview Questions & Answers from Career Guru](http://career.guru99.com/top-50-mysql-interview-questions-answers/)

##### Oracle

* [General Oracle Interview Questions & Answers](http://www.coolinterview.com/type.asp?iType=57)

##### SQL

* [10 Frequently asked SQL Query Interview Questions](http://java67.blogspot.com.by/2013/04/10-frequently-asked-sql-query-interview-questions-answers-database.html)
* [45 Essential SQL Interview Questions from Toptal](http://www.toptal.com/sql/interview-questions)
* [Common Interview Questions and Answers](http://www.indiabix.com/technical/sql-server-common-questions/)
* [General Interview Questions and Answers](http://www.indiabix.com/technical/sql-server-general-questions/)
* [Schema, Questions & Solutions for SQL Exercising](https://github.com/XD-DENG/SQL-exercise)
* [SQL Interview Questions that have been designed specially to get you acquainted with the nature of questions you may encounter during your interview for the subject of SQL](http://www.tutorialspoint.com/sql/sql_interview_questions.htm)
* [SQL Interview Questions CHEAT SHEET](https://www.interviewbit.com/sql-interview-questions/)
* [SQL Journaldev Questions](https://www.journaldev.com/17773/sql-interview-questions-answers)
* [SQL 50 Popular SQL Interview Questions for Testers](https://www.softwaretestinghelp.com/50-popular-sql-interview-questions-for-testers/)
* [10 Frequently Asked SQL Query Interview Questions Answers](https://www.java67.com/2013/04/10-frequently-asked-sql-query-interview-questions-answers-database.html)
* [GeeksforGeeks SQL Interview Questions](https://www.geeksforgeeks.org/sql-interview-questions/)
* [50 SQL Query Questions and Answers for Practice](https://www.techbeamers.com/sql-query-questions-answers-for-practice/)
* [SQL Queries for Interview](https://artoftesting.com/interviewSection/sql-queries-for-interview.html)

##### SQL Lite

* <b>Explain what is SQLite?</b></br>
SQLite is a mostly ACID compliant relational database management system contained in a relatively
small C programming library.

* <b>List out the standard SQLite commands?</b></br>
The standard SQLite commands interact with relational databases are similar to SQL. They are
 * SELECT
 * CREATE
 * INSERT
 * UPDATE
 * DROP
 * DELETE
Based on their operational nature these commands can be classified.

* <b>Explain what is SQLite transactions?</b></br>
The transaction is referred as a unit of work that is performed against a database. It is the
propagation of one or more changes to the database. Properties of transactions are determined by
ACID.
 * Atomicity: It ensures that all work unit are successfully completed
 * Consistency: It ensures that the database changes states upon a successfully committed
transaction
 * Isolation: It enables transactions to operate independently of and transparent to each other
 * Durability: It ensures that the result or effect of a committed transaction persists in case of a
system failure

* <b>List out the areas where SQLite works well?</b></br>
SQLite works well with
 * Embedded devices and the internet of things
 * Application file format
 * Data Analysis
 * Websites
 * Cache for enterprise data
 * Server side database
 * File archives
 * Internal or temporary databases
 * Replacement for ad hoc disk files
 * Experimental SQL language extensions
 * Stand-in for an enterprise database during demos or testing

* <b>What is the difference between SQL and SQLite?</b></br>

<b>SQL</b>
 * SQL is a Structured Query Language
 * SQL support stored procedures
 * SQL is server based

<b>SQLite</b>
 * SQLite is a powerful, embedded  relational database management system mostly used in mobile devices for data storage
 * SQLite does not support stored procedures
 * SQLite is file based

* <b>List out the advantages of SQLite?</b></br>
 * It does not require separate server processor system to operate
 * No setup or administration required SQlite comes with zero-configuration
 * An SQLite database can be stored in a single cross-platform disk file
 * SQLite is very compact less than 400 KiB
 * SQLite is self-contained, which means no external dependencies
 * It supports almost all types of O.S
 * It is written in ANSI-C and provides easy to use API

* <b>Mention what are the SQLite storage classes?</b></br>
SQLite storage classes include
 * Null: The value is a NULL value
 * Integer: The value is a signed integer (1,2,3, etc.)
 * Real: The value is a floating point value, stored as an 8 byte IEEE floating point number
 * Text: The value is a text string, stored using the database encoding ( UTF-8, UTF-16BE)
 * BLOB (Binary Large Object): The value is a blob of data, exactly stored as it was input

* <b>Explain how Boolean values in SQLite are stored?</b></br>
Boolean values in SQLite are stored as integers 0 (false) and 1 (true). SQLite does not have a separate Boolean storage class.

* <b>Explain what is the use of SQLITE group by clause?</b></br>
The SQLITE group by clause is used in collaboration with the SELECT statement to arrange identical
data into groups.

* <b>Mention what is the command used to create a database in SQLite?</b></br>
To create a database in SQLite- command “sqlite3” is used. The basic syntax to create a database is
`$sqlite3 DatabaseName.db`

* <b>Mention what is .dump command is used for?</b></br>
The .dump command is used to make an SQLite database dump, remember once you use the dump command all your data will be dumped forever and cannot be retrieved.

* <b>Explain how can you delete or add columns from an existing table in SQLite?</b></br>
There is a very limited support for alter ( add or delete ) table. In case if you want to delete or add columns from an existing table in SQLite you have to first save the existing data to a temporary table, drop the old table or column, create the new table and then copy the data back in from the temporary table.

* <b>Mention what is the maximum size of a VARCHAR in SQLite?</b></br>
SQLite does not have any specific length for VARCHAR. For instance, you can declare a VARCHAR (10) and SQLite will store a 500 million character string there. It will keep all 500 characters intact.

* <b>Mention when to use SQLite and when not to use SQLite?</b></br>

SQLite can be used in following conditions
 * Embedded applications: Does not require expansion like mobile applications or games
 * Disk assess replacement: Application that require to write or read files to disk directly
 * Testing: When testing business application logic

When not to use SQLite
 * Multi-user applications: Where multiple client needs to access and use same database
 * Applications requiring high write volumes: It enables you to use only one single write operation to take place at any given time

* <b>Explain how to recover deleted data from my SQLite database?</b></br>
To recover the information you can use your backup copy of your database file, but if you do not have a backup copy, then recovery is impossible. SQLite uses SQLITE SECURE DELETE option which overwrites all deleted content with zeroes.

* <b>When can you get an SQLITE_SCHEMA error?</b></br>
The SQLITE_SCHEMA error is returned when a prepared SQL statement is not valid and cannot be executed. Such type occurs only when using the sqlite3 prepare() and sqlite3 step() interfaces to run SQL.

* <b>Mention what is the Export Control Classification Number (EECN) for SQLite?</b></br>
The core public domain SQLite source code is not described by any ECCN. Hence, the ECCN should be reported as EAR99. But if you are adding new code or linking SQLite with the application, then it might change the EECN number.

* <b>Explain what is view in SQLite?</b></br>
In SQLite, a view is actually a composition of a table in the form of pre-defined SQLite Query. A view can consist of all rows of a table or selected rows from one or more tables.

* <b>Explain what are SQLite Indexes?</b></br>
SQLite indexes are special lookup tables that the database search engine use to speed up data retrieval. In simple words, it is a pointer to data in a table.

* <b>When Indexes should be avoided?</b></br>
Indexes should be avoided when
 * Tables are small
 * Tables that changes frequently
 * Columns that are frequently manipulated or having a high number of NULL values

Read more:
* [Top 20 SQL LITE  Interview Questions from Career Guru](http://career.guru99.com/top-20-sql-lite-interview-questions/)
