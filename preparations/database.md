## Contents

* [Basic Questions](#basic-questions)
* [MySQL](#mysql)
* [Oracle](#oracle)
* [SQL](#sql)
* [SQLite](#sqlite)
* [Collection](#collection)
* [Read More](#read-more)

### Basic Questions

### MySQL

* <b>What is Database?</b></br>

  A database is an organized collection of data, stored and retrieved digitally from a remote or local computer system. Databases can be vast and complex, and such databases are developed using fixed design and modeling approaches.

* <b>Define SQL</b></br>

  SQL stands for Structured Query Language. SQL is a programming Language designed specially for managing data in Relational Database Management System (RDBMS).

* <b>About MySQL</b>

  MySQL is an open-source relational database management system (RDBMS). The name is derived from a combination of “My” which stands for the name of the daughter of the co-founder Michael Widenius, and “SQL” which is stands for Structured Query Language.

  MySQL is owned by Oracle, though initially owned and sponsored by a single for-profit firm, the Swedish company MYSQLAB. The MYSQL development project makes its source code accessible under the GNU General Public License terms, including a range of propriety agreements. You can get various paid editions with additional functionality for propriety use.

* <b>What is RDBMS? How is it different from DBMS?</b></br>

  RDBMS stands for Relational Database Management System. The key difference here, compared to DBMS, is that RDBMS stores data in the form of a collection of tables and relations can be defined between the common fields of these tables. Most modern database management systems like MySQL, Microsoft SQL Server, Oracle, IBM DB2 and Amazon Redshift are based on RDBMS.

* <b>What is MySQL?</b></br>

  MySQL is a multithreaded, multi-user SQL database management system which has more than 11 million installations. This is the world's second most popular and widely used open source database. It is interesting how MySQL name was given to this query language. The term My is coined by the name of the daughter of co-founder Michael Widenius's daughter, and SQL is the short form of Structured Query Language. Using MySQL is free of cost for the developer, but enterprises have to pay a license fee to Oracle.

  Formerly MySQL was initially owned by a for-profit firm MySQL AB, then Sun Microsystems bought it and then Oracle bought Sun Microsystems, so Oracle currently owns MySQL.

  MySQL is an Oracle-supported Relational Database Management System (RDBMS) which is based on structured query language. MySQL supports wide ranges of operating systems most famous of those include Windows, Linux & UNIX. Although it is possible to develop a wide range of application with MySQL, it is only used for web applications & online publishing. It is a fundamental part of an open source enterprise known as Lamp.

* <b>What is Lamp?</b>

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


* <b>What is RDBMS? Explain its features?</b></br>

  A Relational Database Management System (RDBMS) is the most widely used database Management System based on the Relational Database model.</br>
  Features of RDBMS:

  * Stores data in tables.
  * Tables have rows and column.
  * Creation and Retrieval of Table is allowed through SQL.


* <b>What is the difference between MySQL and SQL?</b></br>

  * SQL is known as the standard query language. It is used to interact with the database like MySQL. MySQL is a database that stores various types of data and keeps it safe.

  * A PHP script is required to store and retrieve the values inside the database.

  * SQL is a computer language, whereas MySQL is a software or an application

  * SQL is used for the creation of database management systems whereas MySQL is used to enable data handling, storing, deleting and modifying data

* <b>Why do we use the MySQL database server?</b></br>

  * First of all MYSQL server is free to use for developers and a small fee for enterprises.

  * MySQL server is open source.

  * The community of MySQL is tremendous and supportive hence any help regarding MySQL is resolved as soon as possible.

  * MySQL has very stable versions available, as MySQL has been in the market since a long time so all bugs arising in the previous builds have been continuously removed and a very stable version is provided after every update.

  * The MySQL database server is very fast, reliable and easy to use. You can easily use and modify the software. MySQL software can be downloaded free of cost from the internet.

* <b>What is Data Mining?</b></br>

  Data Mining is a subcategory of Computer Science which aims at extraction of information from set of data and transform it into Human Readable structure, to be used later.

* <b>What is an ERD?</b></br>

  ERD stands for Entity Relationship Diagram. Entity Relationship Diagram is the graphical representation of tables, with the relationship between them.

* <b>What is the difference between Primary Key and Unique Key?</b></br>

  Both Primary and Unique Key is implemented for Uniqueness of the column. Primary Key creates a clustered index of column where as an  Unique creates unclustered index of column. Moreover, Primary Key doesn’t allow NULL value, however Unique Key does allows one NULL value.

* <b>What are different types of keys in SQL?</b></br>

  Keys are a vital feature in RDMS, they are essentially fields that link one table to another and promote fast data retrieval and logging through managing column indexes.

  Different types of keys are:

  **Primary Key** – a unique key that identifies records in database tables. By unique it means that it must not be Null and must be unique in the table.

  **Candidate Key** – a unique field which identifies for column or group of columns independently, without any required reference to other fields.

  **Alternate Key** – can be substituted in use for Primary Keys but are considered as a secondary. The difference is that Alternate Keys can have a Null value, provided that the columns have data within them. A type of Candidate Key which is also required to be unique.

  **Unique Key** – Keys that offer restriction to prevent duplicate data within rows except for null entries.

  The other keys available are Foreign Keys, Super Keys, and Composite Keys.

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

  * HEAP tables are found in memory.
  * They are used for high speed storage on temporary basis.

  Some of their characteristics are:
   * They do not allow BLOB or TEXT fields.
   * Only comparison operators like =, <, >, = >, =< can be used with them.
   * AUTO_INCREMENT is not supported by HEAP tables
   * Indexes should be NOT NULL


* <b>How do you control the max size of a HEAP table?</b></br>

  Maximum size of Heap table can be controlled using MySQL config variable called `max_heap_table_size`.

* <b>What are the advantages of MySQL in comparison to Oracle?</b></br>

  * MySQL is a free, fast, reliable, open source relational database while Oracle is expensive, although they have provided Oracle free edition to attract MySQL users.
  * It is portable.
  * GUI with command prompt.
  * Administration is supported by MySQL Query Browser.
  * MySQL uses only just under 1 MB of RAM on your laptop while Oracle 9i installation uses 128 MB.
  * MySQL is great for database enabled websites while Oracle is made for enterprises.


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
  * ‘.frm’ file – storing the table definition
  * ‘.MYD’ (MYData) - data file
  * ‘.MYI’ (MYIndex) – index file

* <b>Explain advantages of MyISAM over InnoDB?</b></br>

  * MyISAM follows a much more conservative approach to disk space management.
  * Storing each MyISAM table in a separate file, which can be further compresses, if required.
  * InnoDB stores the tables in tablespace. Further optimization is difficult with them.


* <b>How can we convert between Unix & MySQL timestamps?</b></br>

  * MySQL timestamp can be converted into Unix timestamp using the command UNIX_TIMESTAMP.
  * Unix timestamp can be converted into MySQL timestamp using the command FROM_UNIXTIME.

* <b>What, if a table has one column defined as TIMESTAMP?</b></br>

  Timestamp field gets the current timestamp whenever the row gets altered.

* <b>What happens when the column is set to AUTO INCREMENT and if you reach maximum value in the table?</b></br>

  It stops incrementing. Any further inserts are going to produce an error, since the key has been used already.

* <b>How can we find out which auto increment was assigned on Last insert?</b></br>

  LAST_INSERT_ID will return the last value assigned by Auto_increment and it is not required to specify the table name.

* <b>How can you see all indexes defined for a table?</b></br>

  Indexes are defined for the table by:</br>
  `SHOW INDEX FROM <tablename>;`

* <b>What is BLOB?</b></br>

  * BLOB stands for binary large object.
  * It that can hold a variable amount of data.

  There are four types of BLOB based on the maximum length of values they can hold:

  * TINYBLOB
  * BLOB
  * MEDIUMBLOB
  * LONGBLOB

* <b>What is TEXT(Non-Standard string types)?</b></br>

  TEXT is case-insensitive BLOB. The four types of TEXT are:

  * TINYTEXT
  * TEXT
  * MEDIUMTEXT
  * LONGTEXT

* <b>What is the difference between BLOB and TEXT?</b></br>

  * In BLOB sorting and comparison is performed in case-sensitive for BLOB values.
  * In TEXT types sorting and comparison is performed case-insensitive.

* <b>How would you enter Characters as HEX Numbers?</b></br>

  * To enter characters as HEX numbers, you can enter HEX numbers with single quotes and a prefix of (X).
  * Alternatively, just prefix HEX numbers with (Ox).

* <b>How will you export tables as an XML file in MySQL?</b></br>

  MYSQL’s query browser has a provision called “Export Result Set” which allows the tables to be exported as XML.

* <b>What is the use of `i-am-a-dummy` flag in MySQL?</b></br>

  Using the i-am-dummy flag makes the SQL engine refuse any Updates or deletes to execute if the WHERE clause is not present. It is very useful when using delete statements. Using i-am-dummy flag will not allow the following statement to execute:</br>
 `Delete from employee;`

* <b>What are the differences between MySQL_fetch_array(), MySQL_fetch_object(), MySQL_fetch_row()?</b></br>

  Mysql_fetch_object returns the result from the database as objects while mysql_fetch_array returns result as an array. This will allow access to the data by the field names.

  E.g. using mysql_fetch_object field can be accessed as $result->name and using mysql_fetch_array field can be accessed as $result->[name]. mysql_fetch_row($result):- where $result is the result resource returned from a successful query executed using the mysql_query() function.

  ```SQL
  $result = mysql_query("SELECT * from students");
  while($row = mysql_fetch_row($result))
  {
        Some statement;
  }
   ```
* <b>What is difference between mysql_connect and mysql_pconnect?</b></br>

  Mysql_connect() opens a new connection to the database while mysql_pconnect() opens a persistent connection to the database. This means that each time the page is loaded mysql_pconnect() does not open the database. Mysql_close() cannot be used to close the persistent connection. Though it can be used to close mysql_connect().

  Mysql_connect:

  * Opens a new connection to the database.
  * The database connection can be closed.
  * Opens the page every time the page is loaded.

  Mysql_pconnect:

  * Opens a persistent connection to the database.
  * The database connection can not be closed.
  * The page need not be opened every time the page is loaded.


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

  Example:</br>
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

  ```SQL
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

  * .frm file consists of the table definition that are stored in the database
  * .myd is an extension that is used by a data file.
  * .myi is an extension that is used by index file.


* <b>What is the difference between MYSQL and SQL?</b></br>

  * SQL is known as standard query language, as the name implies it is the language which is used to interact with the database like MySQL.

  * MySQL is a database that store various types of data and keep it safe. A PHP script is required to store and retrieve the values inside the database.

* <b>How database are managed?</b></br>

  Database is a collection of data and it is managed by a database server, which is a special program that is also known as MySQL database server. Application that you create usually communicates with the database server in the language which it can understand; mostly SQL language is used for communication. Database server in return interacts with the web server on same server or computer. Database server and web server result in the data which is being shown on the web.

* <b>Why phpMyAdmin is used for MYSQL?</b></br>

  PhpMyAdmin is a very popular and easy to use GUI tool that can allow SQL commands to be run to create database, create tables, insert data and retrieve it. It provides a web based interface to the user for the ease of use. phpMyAdmin allows user to manage everything from one place and no other installation is required in the computer after this.

* <b>What is the difference between a database and a table?</b></br>

  There is a major difference between a database and a table. The differences are as follows:

  1. Tables are a way to represent the division of data in a database. Whereas, database is a collection of tables and data.
  2. Tables group the data in relation with each other and create a dataset; this dataset will be used in the database. The data which are stored in the table in any form is a part of the database, but opposite is not true.

* <b>What is the difference between truncate and delete?</b></br>

  Delete command is used to delete data from a table for example Remove emails where we write a script to delete the customer’s data. It deletes the rows of data from a table. The syntax of it as follows:</br>
  `DELETE FROM table_name`

  Whereas, truncate is very dangerous command and should be used carefully as it deletes every row from a table. The syntax of it as follows:</br>
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

  If the values in the column of a table are repeating and a unique value has to be found then the following command can be used in the query:</br>
  `SELECT DISTINCT user_firstname FROM users;`

  There is another command which can be used to find the command to see the distinct values as:</br>
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

  * Heap tables are found in memory. They are used for high-speed storage on a temporary basis. They do not allow BLOB or TEXT fields.

  * Heap tables do not support AUTO_INCREMENT.

  * Indexes should be NOT NULL.

  <b>Temporary tables:</b>

  * The temporary tables are used to keep the transient data. Sometimes it is beneficial in cases to hold temporary data. The Temporary table is deleted after the current client session terminates.

  <b>Main differences:</b>

  * The heap tables are shared among clients while temporary tables are not shared.

  * Heap tables are just another storage engine, while for temporary tables you need a special privilege (create temporary table).

* <b>How to get the current date in MySQL?</b></br>

  To get current date, use the following syntax:</br>
  `SELECT CURRENT_DATE();`  

* <b>What are the security alerts while using MySQL?</b></br>

  * Install antivirus and configure the operating system's firewall.
  * Never use the MySQL Server as the UNIX root user.
  * Change root username and password Restrict or disable remote access.

* <b>How to display Nth highest salary from a table in a MySQL query?</b></br>

  Let us take a table named the employee.
  To find Nth highest salary is:</br>
  `select distinct(salary)from employee order by salary desc limit n-1,1`

  If you want to find 3rd largest salary:</br>
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

  `SELECT * FROM table_name LIMIT 0,20;`

* <b>What is save point in MySQL?</b></br>

  * A defined point in any transaction is known as savepoint.

  * SAVEPOINT is a statement in MySQL which is used to set a named transaction save point with a name of identifier.

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
  ```SQL
  mysql;
  mysql mysql.out;
  ```
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

  Majorly SQL commands can be divided into three categories i.e. DDL, DML & DCL.

  * Data Definition Language (DDL) deals with all the database schemas, and it defines how the data should reside in the database. Commands like Create TABLE and ALTER TABLE are part of DDL.

  * Data Manipulative Language (DML) deals with operations and manipulations on the data the commands in DML are Insert, Select etc.

  * Data Control Languages (DCL) are related to the Grant and permissions. In short, the authorization to access any part of database is defined by these.

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

</br><b>Read more</b>:
* [10 MySQL Database Interview Questions for Beginners and Intermediates](http://www.tecmint.com/10-mysql-database-interview-questions-for-beginners-and-intermediates/)
* [100 MySQL interview questions](http://www.careerride.com/MySQL-Interview-Questions.aspx)
* [15 Basic MySQL Interview Questions for Database Administrators](http://www.tecmint.com/basic-mysql-interview-questions-for-database-administrators/)
* [28 MySQL interview questions from JavaTPoint.com](http://www.javatpoint.com/mysql-interview-questions)
* [40 Basic MySQL Interview Questions with Answers](http://www.testingbrain.com/interview/mysql-interview-questions.html)
* [Top 50 MySQL Interview Questions & Answers from Career Guru](http://career.guru99.com/top-50-mysql-interview-questions-answers/)

### Oracle

* [General Oracle Interview Questions & Answers](http://www.coolinterview.com/type.asp?iType=57)

### SQL

* <b>SQL Query to find second highest salary of Employee.</b></br>

  There are many ways to find second highest salary of Employee in SQL, you can either use SQL Join or Subquery to solve this problem. Here is SQL query using Subquery:
  `select MAX(Salary) from Employee WHERE Salary NOT IN (select MAX(Salary) from Employee ); `
  Read more: [Java Revisited](https://javarevisited.blogspot.com/2012/12/how-to-find-second-highest-or-maximum-salary-sql.html)

* <b>SQL Query to find Max Salary from each department.</b></br>

  You can find the maximum salary for each department by grouping all records by DeptId and then using MAX() function to calculate maximum salary in each group or each department.</br>
  `SELECT DeptID, MAX(Salary) FROM Employee  GROUP BY DeptID. `</br>
  These questions become more interesting if Interviewer will ask you to print department name instead of department id, in that case, you need to join Employee table with Department using foreign key DeptID, make sure you do LEFT or RIGHT OUTER JOIN to include departments without any employee as well.  Here is the query.</br>
  `SELECT DeptName, MAX(Salary) FROM Employee e RIGHT JOIN Department d ON e.DeptId = d.DeptID GROUP BY DeptName;`</br>
  In this query, we have used RIGHT OUTER JOIN because we need the name of the department from Department table which is on the right side of JOIN clause, even if there is no reference of dept_id on Employee table.

* <b>Write SQL Query to display the current date.</b></br>

  SQL has built-in function called GetDate() which returns the current timestamp. This will work in Microsoft SQL Server, other vendors like Oracle and MySQL also has equivalent functions.</br>
  `SELECT GetDate(); `

* <b>Write an SQL Query to check whether date passed to Query is the date of given format or not.</b></br>

  SQL has IsDate() function which is used to check passed value is a date or not of specified format, it returns 1(true) or 0(false) accordingly. Remember ISDATE() is an MSSQL function and it may not work on Oracle, MySQL or any other database but there would be something similar.</br>
  `SELECT  ISDATE('1/08/13') AS "MM/DD/YY";`</br>
  It will return 0 because passed date is not in correct format.

* <b>Write an SQL Query to print the name of the distinct employee whose DOB is between 01/01/1960 to 31/12/1975.</b></br>

  This SQL query is tricky, but you can use BETWEEN clause to get all records whose date fall between two dates.</br>
  `SELECT DISTINCT EmpName FROM Employees WHERE DOB  BETWEEN ‘01/01/1960’ AND ‘31/12/1975’;`

* <b>Write an SQL Query find number of employees according to gender  whose DOB is between 01/01/1960 to 31/12/1975.</b></br>

  `SELECT COUNT(\*), sex from Employees  WHERE  DOB BETWEEN '01/01/1960' AND '31/12/1975'  GROUP BY sex;`

* <b>Write an SQL Query to find an employee whose Salary is equal or greater than 10000.</b></br>

  `SELECT EmpName FROM  Employees WHERE  Salary>=10000;`

* <b>Write an SQL Query to find name of employee whose name Start with ‘M’</b></br>

  `SELECT * FROM Employees WHERE EmpName like 'M%';`

* <b>find all Employee records containing the word "Joe", regardless of whether it was stored as JOE, Joe, or joe.</b></br>

  `SELECT * from Employees  WHERE  UPPER(EmpName) like '%JOE%';`

* <b>Write an SQL Query to find  the year from date.</b></br>

  Here is how you can find Year from a Date in SQL Server 2008 .
  `SELECT YEAR(GETDATE()) as "Year";`

* <b> Write SQL Query to find duplicate rows in a database? and then write SQL query to delete them?</b></br>

  You can use the following query to select distinct records:</br>
  `SELECT * FROM emp a WHERE rowid = (SELECT MAX(rowid) FROM EMP b WHERE a.empno=b.empno)`

* <b>Write SQL Query to find duplicate rows in a database? and then write SQL query to delete them?</b></br>

  You can use the following query to select distinct records:</br>
  `SELECT * FROM emp a WHERE rowid = (SELECT MAX(rowid) FROM EMP b WHERE a.empno=b.empno)`

  To delete:</br>
  `DELETE FROM emp a WHERE rowid != (SELECT MAX(rowid) FROM emp b WHERE a.empno=b.empno);`

* <b>There is a table which contains two column Student and Marks, you need to find all the students, whose marks are greater than average marks i.e. list of above average students.</b></br>

  This query can be written using subquery as shown below:</br>
  `SELECT student, marks from table where marks > SELECT AVG(marks) from table) `</br>
  ![SQL Schema](/image%20assets/database_preparation_2.png)

* <b>How do you find all employees which are also manager?</b></br>

  Note: You have given a standard employee table with an additional column mgr_id, which contains employee id of the manager.</br>
  ![Employee Manager](/image%20assets/database_preparation_1.png)</br>
  Answer: You need to know about self-join to solve this problem. In Self Join, you can join two instances of the same table to find out additional details as shown below</br>
  `SELECT e.name, m.name FROM Employee e, Employee m WHERE e.mgr_id = m.emp_id; `

  this will show employee name and manager name in two column e.g.

  name  manager_name
  John   David

  One follow-up is to modify this query to include employees which don't have a manager. To solve that, instead of using the inner join, just use left outer join, this will also include employees without managers.

* <b>You have a composite index of three columns, and you only provide the value of two columns in WHERE clause of a select query? Will Index be used for this operation?</b>For example if Index is on EmpId, EmpFirstName, and EmpSecondName and you write query like</br>

  `SELECT * FROM Employee WHERE EmpId=2 and EmpFirstName='Radhe'`

  If the given two columns are secondary index column then the index will not invoke, but if the given 2 columns contain the primary index(first column while creating index) then the index will invoke. In this case, Index will be used because EmpId and EmpFirstName are primary columns.

* <b>What does `UNION` do? What is the difference between `UNION` and `UNION ALL`?</b></br>

  UNION merges the contents of two structurally-compatible tables into a single combined table. The difference between UNION and UNION ALL is that UNION will omit duplicate records whereas UNION ALL will include duplicate records.

  It is important to note that the performance of UNION ALL will typically be better than UNION, since UNION requires the server to do the additional work of removing any duplicates. So, in cases where is is certain that there will not be any duplicates, or where having duplicates is not a problem, use of UNION ALL would be recommended for performance reasons.

* <b>List and explain the different types of JOIN clauses supported in ANSI-standard SQL.</b></br>

  ANSI-standard SQL specifies five types of JOIN clauses as follows:

  * INNER JOIN (a.k.a. “simple join”): Returns all rows for which there is at least one match in BOTH tables. This is the default type of join if no specific JOIN type is specified.

  * LEFT JOIN (or LEFT OUTER JOIN): Returns all rows from the left table, and the matched rows from the right table; i.e., the results will contain all records from the left table, even if the JOIN condition doesn’t find any matching records in the right table. This means that if the ON clause doesn’t match any records in the right table, the JOIN will still return a row in the result for that record in the left table, but with NULL in each column from the right table.

  * RIGHT JOIN (or RIGHT OUTER JOIN): Returns all rows from the right table, and the matched rows from the left table. This is the exact opposite of a LEFT JOIN; i.e., the results will contain all records from the right table, even if the JOIN condition doesn’t find any matching records in the left table. This means that if the ON clause doesn’t match any records in the left table, the JOIN will still return a row in the result for that record in the right table, but with NULL in each column from the left table.

  * FULL JOIN (or FULL OUTER JOIN): Returns all rows for which there is a match in EITHER of the tables. Conceptually, a FULL JOIN combines the effect of applying both a LEFT JOIN and a RIGHT JOIN; i.e., its result set is equivalent to performing a UNION of the results of left and right outer queries.

  * CROSS JOIN: Returns all records where each row from the first table is combined with each row from the second table (i.e., returns the Cartesian product of the sets of rows from the joined tables). Note that a CROSS JOIN can either be specified using the CROSS JOIN syntax (“explicit join notation”) or (b) listing the tables in the FROM clause separated by commas without using a WHERE clause to supply join criteria (“implicit join notation”).

  * Self Join This is a particular case when one table joins to itself, with one or two aliases to avoid confusion. A self join can be of any type, as long as the joined tables are the same. A self join is rather unique in that it involves a relationship with only one table. The common example is when company has a hierarchal reporting structure whereby one member of staff reports to another. Self Join can be Outer Join or Inner Join.

* <b>Write a SQL query using UNION ALL (not UNION) that uses the WHERE clause to eliminate duplicates. Why might you want to do this?</b></br>

  You can avoid duplicates using UNION ALL and still run much faster than UNION DISTINCT (which is actually same as UNION) by running a query like this:

  `SELECT * FROM mytable WHERE a=X UNION ALL SELECT * FROM mytable WHERE b=Y AND a!=X`
  The key is the AND a!=X part. This gives you the benefits of the UNION (a.k.a., UNION DISTINCT) command, while avoiding much of its performance hit.

* <b>What is an execution plan? When would you use it? How would you view the execution plan?</b></br>

  An execution plan is basically a road map that graphically or textually shows the data retrieval methods chosen by the SQL server’s query optimizer for a stored procedure or ad hoc query. Execution plans are very useful for helping a developer understand and analyze the performance characteristics of a query or stored procedure, since the plan is used to execute the query or stored procedure.

  In many SQL systems, a textual execution plan can be obtained using a keyword such as EXPLAIN, and visual representations can often be obtained as well. In Microsoft SQL Server, the Query Analyzer has an option called “Show Execution Plan” (located on the Query drop down menu). If this option is turned on, it will display query execution plans in a separate window when a query is run.

* <b>List and explain each of the ACID properties that collectively guarantee that database transactions are processed reliably.</b></br>

  ACID (Atomicity, Consistency, Isolation, Durability) is a set of properties that guarantee that database transactions are processed reliably. They are defined as follows:

  * Atomicity. Atomicity requires that each transaction be “all or nothing”: if one part of the transaction fails, the entire transaction fails, and the database state is left unchanged. An atomic system must guarantee atomicity in each and every situation, including power failures, errors, and crashes.
  * Consistency. The consistency property ensures that any transaction will bring the database from one valid state to another. Any data written to the database must be valid according to all defined rules, including constraints, cascades, triggers, and any combination thereof.
  * Isolation. The isolation property ensures that the concurrent execution of transactions results in a system state that would be obtained if transactions were executed serially, i.e., one after the other. Providing isolation is the main goal of concurrency control. Depending on concurrency control method (i.e. if it uses strict - as opposed to relaxed - serializability), the effects of an incomplete transaction might not even be visible to another transaction.
  * Durability. Durability means that once a transaction has been committed, it will remain so, even in the event of power loss, crashes, or errors. In a relational database, for instance, once a group of SQL statements execute, the results need to be stored permanently (even if the database crashes immediately thereafter). To defend against power loss, transactions (or their effects) must be recorded in a non-volatile memory.

* <b>How can you select all the even number records from a table? All the odd number records?</b></br>

  To select all the even number records from a table:

  `Select * from table where id % 2 = 0`
  To select all the odd number records from a table:

  `Select * from table where id % 2 != 0`

* <b>What are the NVL and the NVL2 functions in SQL? How do they differ?</b></br>

  Both the NVL(exp1, exp2) and NVL2(exp1, exp2, exp3) functions check the value exp1 to see if it is null.

  With the NVL(exp1, exp2) function, if exp1 is not null, then the value of exp1 is returned; otherwise, the value of exp2 is returned, but case to the same data type as that of exp1.

  With the NVL2(exp1, exp2, exp3) function, if exp1 is not null, then exp2 is returned; otherwise, the value of exp3 is returned.

* <b>What is the purpose of the NVL function?</b></br>

  The NVL function converts a NULL value to an actual value.

* <b>What is the difference between the RANK() and DENSE_RANK() functions? Provide an example.</b></br>

  The only difference between the RANK() and DENSE_RANK() functions is in cases where there is a “tie”; i.e., in cases where multiple values in a set have the same ranking. In such cases, RANK() will assign non-consecutive “ranks” to the values in the set (resulting in gaps between the integer ranking values when there is a tie), whereas DENSE_RANK() will assign consecutive ranks to the values in the set (so there will be no gaps between the integer ranking values in the case of a tie).

  For example, consider the set {25, 25, 50, 75, 75, 100}. For such a set, RANK() will return {1, 1, 3, 4, 4, 6} (note that the values 2 and 5 are skipped), whereas DENSE_RANK() will return {1,1,2,3,3,4}.

* <b>What is the difference between the WHERE and HAVING clauses?</b></br>

  When GROUP BY is not used, the WHERE and HAVING clauses are essentially equivalent.

  However, when GROUP BYis used:

  * The WHERE clause is used to filter records from a result. The filtering occurs before any groupings are made.
  * The HAVING clause is used to filter values from a group (i.e., to check conditions after aggregation into groups has been performed).

* <b>What is the difference between char and varchar2?</b></br>

  When stored in a database, varchar2 uses only the allocated space. E.g. if you have a varchar2(1999) and put 50 bytes in the table, it will use 52 bytes.

  But when stored in a database, char always uses the maximum length and is blank-padded. E.g. if you have char(1999) and put 50 bytes in the table, it will consume 2000 bytes.

* <b>Can we insert a row for identity column implicitly?</b></br>

  Yes, like so:
  ```SQL
  SET IDENTITY_INSERT TABLE1 ON
  INSERT INTO TABLE1 (ID,NAME)
  SELECT ID,NAME FROM TEMPTB1
  SET IDENTITY_INSERT OFF
  ```

* <b>How do you get the last id without the max function?</b></br>

  In MySQL:

  `select id from table order by id desc limit 1`
  In SQL Server:

  `select top 1 id from table order by id desc`

* <b>What is the difference between IN and EXISTS?</b></br>

  IN:

  * Works on List result set
  * Doesn’t work on subqueries resulting in Virtual tables with multiple columns
  * Compares every value in the result list
  * Performance is comparatively SLOW for larger resultset of subquery

  EXISTS:

  * Works on Virtual tables
  * Is used with co-related queries
  * Exits comparison when match is found
  * Performance is comparatively FAST for larger resultset of subquery

* <b>How can you use a CTE to return the fifth highest (or Nth highest) salary from a table?</b></br>

  ```SQL
  Declare @N int
  set @N = 5;
  WITH CTE AS
  (
      SELECT Name, Salary, EmpID, RN = ROW_NUMBER()
	    OVER (ORDER BY Salary DESC)
     FROM Employee
   )
   SELECT Name, Salary, EmpID
   FROM CTE
   WHERE RN = @N
   ```

* <b>How do you get the Nth-highest salary from the Employee table without a subquery or CTE?</b></br>

  `SELECT salary from Employee order by salary DESC LIMIT 2,1`
  This will give the third-highest salary from the Employee table. Accordingly we can find out Nth salary using LIMIT (N-1),1.

  But MS SQL Server doesn’t support that syntax, so in that case:</br>
  ```SQL
  SELECT salary from Employee order by salary DESC
  OFFSET 2 ROWS
  FETCH NEXT 1 ROW ONLY
  OFFSET’s parameter corresponds to the (N-1) above.
  ```

* <b>How do you copy data from one table to another table?</b></br>

  ```SQL
  INSERT INTO table2 (column1, column2, column3, ...)
  SELECT column1, column2, column3, ...
  FROM table1
  WHERE condition;
  ```

* <b>How to find a duplicate record?</b>

  1. Duplicate records with one field

  ```SQL
  SELECT name, COUNT(email)
  FROM users
  GROUP BY email
  HAVING COUNT(email) > 1
  ```
  2. Duplicate records with more than one field

  ```SQL
  SELECT name, email, COUNT(*)
  FROM users
  GROUP BY name, email
  HAVING COUNT(*) > 1
  ```

* <b>Which TCP/IP port does SQL Server run on? How can it be changed?</b></br>

  SQL Server runs on port 1433. It can be changed from the Network Utility TCP/IP properties.

* <b>What are the different index configurations a table can have?</b></br>

  A table can have one of the following index configurations:
  * No indexes
  * A clustered index
  * A clustered index and many nonclustered indexes
  * A nonclustered index
  * Many nonclustered indexes

* <b>What are different types of Collation Sensitivity?</b></br>

  * Case sensitivity - A and a, B and b, etc.
  * Accent sensitivity
  * Kana Sensitivity - When Japanese kana characters Hiragana and Katakana are treated differently, it is called Kana sensitive.
  * Width sensitivity - A single-byte character (half-width) and the same character represented as a double-byte character (full-width) are treated differently than it is width sensitive.

* <b>What is OLTP (Online Transaction Processing)? </b></br>

  In OLTP - online transaction processing systems relational database design use the discipline of data modeling and generally follow the Codd rules of data normalization in order to ensure absolute data integrity. Using these rules complex information is broken down into its most simple structures (a table) where all of the individual atomic level elements relate to each other and satisfy the normalization rules.

* <b>What is Data Integrity?</b></br>

  Data Integrity is the assurance of accuracy and consistency of data over its entire life-cycle, and is a critical aspect to the design, implementation and usage of any system which stores, processes, or retrieves data. It also defines integrity constraints to enforce business rules on the data when it is entered into an application or a database.

* <b>What is difference between DELETE and TRUNCATE commands?</b></br>

  Delete command removes the rows from a table based on the condition that we provide with a WHERE clause. Truncate will actually remove all the rows from a table and there will be no data in the table after we run the truncate command.

  **TRUNCATE:**
  * TRUNCATE is faster and uses fewer system and transaction log resources than DELETE.
  * TRUNCATE removes the data by deallocating the data pages used to store the table's data, and only the page deallocations are recorded in the transaction log.
  * TRUNCATE removes all rows from a table, but the table structure, its columns, constraints, indexes and so on, remains. The counter used by an identity for new rows is reset to the seed for the column.
  * You cannot use TRUNCATE TABLE on a table referenced by a FOREIGN KEY constraint. Because TRUNCATE TABLE is not logged, it cannot activate a trigger.
  * TRUNCATE cannot be rolled back.
  * TRUNCATE is DDL Command.
  * TRUNCATE Resets identity of the table

  **DELETE:**
  * DELETE removes rows one at a time and records an entry in the transaction log for each deleted row.
  * If you want to retain the identity counter, use DELETE instead. If you want to remove table definition and its data, use the DROP TABLE statement.
  * DELETE Can be used with or without a WHERE clause
  * DELETE Activates Triggers.
  * DELETE can be rolled back.
  * DELETE is DML Command.
  * DELETE does not reset identity of the table.

  Note: DELETE and TRUNCATE both can be rolled back when surrounded by TRANSACTION if the current session is not closed. If TRUNCATE is written in Query Editor surrounded by TRANSACTION and if session is closed, it can not be rolled back but DELETE can be rolled back.

* <b>When is the use of UPDATE_STATISTICS command?</b></br>

  This command is basically used when a large processing of data has occurred. If a large amount of deletions any modification or Bulk Copy into the tables has occurred, it has to update the indexes to take these changes into account. UPDATE_STATISTICS updates the indexes on these tables accordingly.

* <b>What are the properties and different Types of Sub-Queries?</b></br>

  **Properties of Sub-Query**
  * A sub-query must be enclosed in the parenthesis.
  * A sub-query must be put in the right hand of the comparison operator, and
  * A sub-query cannot contain an ORDER-BY clause.
  * A query can contain more than one sub-query.

  **Types of Sub-Query**
  * Single-row sub-query, where the sub-query returns only one row.
  * Multiple-row sub-query, where the sub-query returns multiple rows,. and
  * Multiple column sub-query, where the sub-query returns multiple columns

* <b>What is SQL Profiler?</b></br>

  SQL Profiler is a graphical tool that allows system administrators to monitor events in an instance of Microsoft SQL Server. You can capture and save data about each event to a file or SQL Server table to analyze later. For example, you can monitor a production environment to see which stored procedures are hampering performances by executing too slowly.

  Use SQL Profiler to monitor only the events in which you are interested. If traces are becoming too large, you can filter them based on the information you want, so that only a subset of the event data is collected. Monitoring too many events adds overhead to the server and the monitoring process and can cause the trace file or trace table to grow very large, especially when the monitoring process takes place over a long period of time.

* <b>What are the authentication modes in SQL Server? How can it be changed?</b></br>

  Windows mode and Mixed Mode - SQL and Windows. To change authentication mode in SQL Server click Start, Programs, Microsoft SQL Server and click SQL Enterprise Manager to run SQL Enterprise Manager from the Microsoft SQL Server program group. Select the server then from the Tools menu select SQL Server Configuration Properties, and choose the Security page.

* <b>Which command using Query Analyzer will give you the version of SQL server and operating system?</b></br>

  `SELECT SERVERPROPERTY ('productversion'), SERVERPROPERTY ('productlevel'), SERVERPROPERTY ('edition').`

* <b>What is SQL Server Agent?</b></br>

  SQL Server agent plays an important role in the day-to-day tasks of a database administrator (DBA). It is often overlooked as one of the main tools for SQL Server management. Its purpose is to ease the implementation of tasks for the DBA, with its full- function scheduling engine, which allows you to schedule your own jobs and scripts.

* <b>Can a stored procedure call itself or recursive stored procedure? How much level SP nesting is possible?</b></br>

  Yes. Because Transact-SQL supports recursion, you can write stored procedures that call themselves. Recursion can be defined as a method of problem solving wherein the solution is arrived at by repetitively applying it to subsets of the problem. A common application of recursive logic is to perform numeric computations that lend themselves to repetitive evaluation by the same processing steps. Stored procedures are nested when one stored procedure calls another or executes managed code by referencing a CLR routine, type, or aggregate. You can nest stored procedures and managed code references up to 32 levels.

* <b>What is Log Shipping?</b></br>

  Log shipping is the process of automating the backup of database and transaction log files on a production SQL server, and then restoring them onto a standby server. Enterprise Editions only supports log shipping. In log shipping the transactional log file from one server is automatically updated into the backup database on the other server. If one server fails, the other server will have the same db and can be used this as the Disaster Recovery plan. The key feature of log shipping is that it will automatically backup transaction logs throughout the day and automatically restore them on the standby server at defined interval.

* <b>Name 3 ways to get an accurate count of the number of records in a table?</b></br>

  ```SQL
  SELECT * FROM table1
  SELECT COUNT(*) FROM table1
  SELECT rows FROM sysindexes WHERE id = OBJECT_ID(table1) AND indid < 2
  ```

* <b>What does it mean to have QUOTED_IDENTIFIER ON? What are the implications of having it OFF?</b></br>

  When SET QUOTED_IDENTIFIER is ON, identifiers can be delimited by double quotation marks, and literals must be delimited by single quotation marks. When SET QUOTED_IDENTIFIER is OFF, identifiers cannot be quoted and must follow all Transact-SQL rules for identifiers.

* <b>What is the difference between a Local and a Global temporary table?</b></br>

  * A local temporary table exists only for the duration of a connection or, if defined inside a compound statement, for the duration of the compound statement.
  * A global temporary table remains in the database permanently, but the rows exist only within a given connection. When connection is closed, the data in the global temporary table disappears. However, the table definition remains with the database for access when database is opened next time.

* <b>What is the STUFF function and how does it differ from the REPLACE function?</b></br>

  STUFF function is used to overwrite existing characters. Using this syntax, STUFF (string_expression, start, length, replacement_characters), string_expression is the string that will have characters substituted, start is the starting position, length is the number of characters in the string that are substituted, and replacement_characters are the new characters interjected into the string. REPLACE function to replace existing characters of all occurrences. Using the syntax REPLACE (string_expression, search_string, replacement_string), where every incidence of search_string found in the string_expression will be replaced with replacement_string.

* <b>What is PRIMARY KEY?</b></br>

  A PRIMARY KEY constraint is a unique identifier for a row within a database table. Every table should have a primary key constraint to uniquely identify each row and only one primary key constraint can be created for each table. The primary key constraints are used to enforce entity integrity.

* <b>What is UNIQUE KEY constraint?</b></br>

  A UNIQUE constraint enforces the uniqueness of the values in a set of columns, so no duplicate values are entered. The unique key constraints are used to enforce entity integrity as the primary key constraints.

* <b>What is FOREIGN KEY?</b></br>

  A FOREIGN KEY constraint prevents any actions that would destroy links between tables with the corresponding data values. A foreign key in one table points to a primary key in another table. Foreign keys prevent actions that would leave rows with foreign key values when there are no primary keys with that value. The foreign key constraints are used to enforce referential integrity.

* <b>What is CHECK Constraint?</b></br>

  A CHECK constraint is used to limit the values that can be placed in a column. The check constraints are used to enforce domain integrity.

* <b>What is NOT NULL Constraint?</b></br>

  A NOT NULL constraint enforces that the column will not accept null values. The not null constraints are used to enforce domain integrity, as the check constraints.

* <b>How to get @@ERROR and @@ROWCOUNT at the same time?</b></br>

  If @@Rowcount is checked after Error checking statement then it will have 0 as the value of @@Recordcount as it would have been reset. And if @@Recordcount is checked before the error-checking statement then @@Error would get reset. To get @@error and @@rowcount at the same time do both in same statement and store them in local variable.

  `SELECT @RC = @@ROWCOUNT, @ER = @@ERROR`

* <b>What is a Scheduled Jobs or What is a Scheduled Tasks?</b></br>

  Scheduled tasks let user automate processes that run on regular or predictable cycles. User can schedule administrative tasks, such as cube processing, to run during times of slow business activity. User can also determine the order in which tasks run by creating job steps within a SQL Server Agent job. E.g. back up database, Update Stats of Tables. Job steps give user control over flow of execution. If one job fails, user can configure SQL Server Agent to continue to run the remaining tasks or to stop execution.

* <b>What are the advantages of using Stored Procedures?</b></br>

  * Stored procedure can reduced network traffic and latency, boosting application performance.
  * Stored procedure execution plans can be reused, staying cached in SQL Server's memory, reducing server overhead.
  * Stored procedures help promote code reuse.
  * Stored procedures can encapsulate logic. You can change stored procedure code without affecting clients.
  * Stored procedures provide better security to your data.

* <b>What is Hibernate and its relation to SQL?</b></br>

  Hibernate is Object Relational Mapping tool in Java. Hibernate let's us write object-oriented code and internally converts them to native SQL queries to execute against a relational database.

  Hibernate uses its own language like SQL which is called Hibernate Query Language(HQL). The difference is that HQL boasts on being able to query Hibernate’s entity objects.

  It also has an object-oriented query language in Hibernate which is called Criteria Query. It proves very beneficial and helpful to developers who primarily use objects in their front-end applications and Criteria Query can cater to those objects in even add SQL-like features such as security and restriction-access.

* <b>How can we solve SQL Error: ORA-00904: invalid identifier?</b></br>

  This error usually appears due to syntax errors on calling a column name in Oracle database, notice the ORA identifier in the error code. Make sure you typed in the correct column name. Also, take special note on the aliases as they are the one being referenced in the error as the invalid identifier.

* <b>What is a table called, if it has neither Cluster nor Non-cluster Index? What is it used for?</b></br>

  Unindexed table or Heap. Microsoft Press Books and Book on Line (BOL) refers it as Heap. A heap is a table that does not have a clustered index and, therefore, the pages are not linked by pointers. The IAM pages are the only structures that link the pages in a table together. Unindexed tables are good for fast storing of data. Many times it is better to drop all indexes from table and then do bulk of inserts and to restore those indexes after that.

* <b>Can SQL Servers linked to other servers like Oracle?</b></br>

  SQL Server can be linked to any server provided it has OLE-DB provider from Microsoft to allow a link. E.g. Oracle has an OLE-DB provider for oracle that Microsoft provides to add it as linked server to SQL Server group.

* <b>What is BCP? When does it used?</b></br>

  BulkCopy is a tool used to copy huge amount of data from tables and views. BCP does not copy the structures same as source to destination. BULK INSERT command helps to import a data file into a database table or view in a user-specified format.

* <b>How to implement one-to-one, one-to-many and many-to-many relationships while designing tables?</b></br>

  One-to-One relationship can be implemented as a single table and rarely as two tables with primary and foreign key relationships. One-to-Many relationships are implemented by splitting the data into two tables with primary key and foreign key relationships. Many-to-Many relationships are implemented using a junction table with the keys from both the tables forming the composite primary key of the junction table.

* <b>What is an execution plan? When would you use it? How would you view the execution plan?</b></br>

  An execution plan is basically a road map that graphically or textually shows the data retrieval methods chosen by the SQL Server query optimizer for a stored procedure or ad- hoc query and is a very useful tool for a developer to understand the performance characteristics of a query or stored procedure since the plan is the one that SQL Server will place in its cache and use to execute the stored procedure or query. From within Query Analyzer is an option called "Show Execution Plan" (located on the Query drop-down menu). If this option is turned on it will display query execution plan in separate window when query is ran again.

* <b>What is RDBMS?</b></br>

  Relational Data Base Management Systems (RDBMS) are database management systems that maintain data records and indices in tables. Relationships may be created and maintained across and among the data and tables. In a relational database, relationships between data items are expressed by means of tables. Interdependencies among these tables are expressed by data values rather than by pointers. This allows a high degree of data independence. An RDBMS has the capability to recombine the data items from different files, providing powerful tools for data usage.

* <b>What are the properties of the Relational tables?</b></br>

  Relational tables have six properties:
  * Values are atomic.
  * Column values are of the same kind.
  * Each row is unique.
  * The sequence of columns is insignificant.
  * The sequence of rows is insignificant.
  * Each column must have a unique name.

* <b>What is Normalization?</b></br>

  Database normalization is a data design and organization process applied to data structures based on rules that help building relational databases. In relational database design, the process of organizing data to minimize redundancy is called normalization. Normalization usually involves dividing a database into two or more tables and defining relationships between the tables. The objective is to isolate data so that additions, deletions, and modifications of a field can be made in just one table and then propagated through the rest of the database via the defined relationships.

* <b>What are different normalization forms?</b></br>

  * 1NF: Eliminate Repeating Groups Make a separate table for each set of related attributes, and give each table a primary key. Each field contains at most one value from its attribute domain.
  * 2NF: Eliminate Redundant Data If an attribute depends on only part of a multi-valued key, remove it to a separate table.
  * 3NF: Eliminate Columns Not Dependent On Key If attributes do not contribute to a description of the key, remove them to a separate table. All attributes must be directly dependent on the primary key.
  * BCNF: Boyce-Codd Normal Form If there are non-trivial dependencies between candidate key attributes, separate them out into distinct tables.
  * 4NF: Isolate Independent Multiple Relationships No table may contain two or more 1:n or n:m relationships that are not directly related.
  * 5NF: Isolate Semantically Related Multiple Relationships There may be practical constrains on information that justify separating logically related many-to-many relationships.
  * ONF: Optimal Normal Form A model limited to only simple (elemental) facts, as expressed in Object Role Model notation.
  * DKNF: Domain-Key Normal Form A model free from all modification anomalies is said to be in DKNF.
Remember, these normalization guidelines are cumulative. For a database to be in 3NF, it must first fulfill all the criteria of a 2NF and 1NF database.

* <b>What is Stored Procedure?</b></br>

  A stored procedure is a named group of SQL statements that have been previously created and stored in the server database. Stored procedures accept input parameters so that a single procedure can be used over the network by several clients using different input data. And when the procedure is modified, all clients automatically get the new version. Stored procedures reduce network traffic and improve performance. Stored procedures can be used to help ensure the integrity of the database.

  e.g. sp_helpdb, sp_renamedb, sp_depends etc.

* <b>What is Nested Trigger?</b></br>

  A trigger can also contain INSERT, UPDATE and DELETE logic within itself, so when the trigger is fired because of data modification it can also cause another data modification, thereby firing another trigger. A trigger that contains data modification logic within itself is called a nested trigger.

* <b>What is View?</b></br>

  A simple view can be thought of as a subset of a table. It can be used for retrieving data, as well as updating or deleting rows. Rows updated or deleted in the view are updated or deleted in the table the view was created with. It should also be noted that as data in the original table changes, so does data in the view, as views are the way to look at part of the original table. The results of using a view are not permanently stored in the database. The data accessed through a view is actually constructed using standard T-SQL select command and can come from one to many different base tables or even other views.

* <b>What is Index?</b></br>

  An index is a physical structure containing pointers to the data. Indices are created in an existing table to locate rows more quickly and efficiently. It is possible to create an index on one or more columns of a table, and each index is given a name. The users cannot see the indexes; they are just used to speed up queries. Effective indexes are one of the best ways to improve performance in a database application. A table scan happens when there is no index available to help a query. In a table scan SQL Server examines every row in the table to satisfy the query results. Table scans are sometimes unavoidable, but on large tables, scans have a terrific impact on performance.

* <b>What is a Linked Server?</b></br>

  Linked Servers is a concept in SQL Server by which we can add other SQL Server to a Group and query both the SQL Server dbs using T-SQL Statements. With a linked server, you can create very clean, easy to follow, SQL statements that allow remote data to be retrieved, joined and combined with local data. Stored Procedure sp_addlinkedserver, sp_addlinkedsrvlogin will be used add new Linked Server.

* <b>What is Cursor?</b></br>

  Cursor is a database object used by applications to manipulate data in a set on a row-by- row basis, instead of the typical SQL commands that operate on all the rows in the set at one time.


  In order to work with a cursor we need to perform some steps in the following order:

  * Declare cursor - DECLARE a cursor after any variable declaration. The cursor declaration must always be associated with a SELECT Statement.
  * Open cursor - Open cursor to initialize the result set. The OPEN statement must be called before fetching rows from the result set.
  * Fetch row from the cursor - FETCH statement to retrieve and move to the next row in the result set.
  * Process fetched row
  * Close cursor - Call the CLOSE statement to deactivate the cursor.
  * Deallocate cursor - Finally use the DEALLOCATE statement to delete the cursor definition and release the associated resources.

* <b>What is Collation?</b></br>

  Collation refers to a set of rules that determine how data is sorted and compared. Character data is sorted using rules that define the correct character sequence, with options for specifying case sensitivity, accent marks, kana character types and character width.

* <b>What is Difference between Function and Stored Procedure?</b></br>

  UDF can be used in the SQL statements anywhere in the WHERE/HAVING/SELECT section where as Stored procedures cannot be. UDFs that return tables can be treated as another rowset. This can be used in JOINs with other tables. Inline UDF's can be thought of as views that take parameters and can be used in JOINs and other Rowset operations.

* <b>What is sub-query? Explain properties of sub-query?</b></br>

  Sub-queries are often referred to as sub-selects, as they allow a SELECT statement to be executed arbitrarily within the body of another SQL statement. A sub-query is executed by enclosing it in a set of parentheses. Sub-queries are generally used to return a single row as an atomic value, though they may be used to compare values against multiple rows with the IN keyword.

  A subquery is a SELECT statement that is nested within another T-SQL statement. A subquery SELECT statement if executed independently of the T-SQL statement, in which it is nested, will return a resultset. Meaning a subquery SELECT statement can standalone and is not depended on the statement in which it is nested. A subquery SELECT statement can return any number of values, and can be found in, the column list of a SELECT statement, a FROM, GROUP BY, HAVING, and/or ORDER BY clauses of a T-SQL statement. A Subquery can also be used as a parameter to a function call. Basically a subquery can be used anywhere an expression can be used.

* <b>What is User Defined Functions? What kind of User-Defined Functions can be created?</b></br>

  User-Defined Functions allow defining its own T-SQL functions that can accept 0 or more parameters and return a single scalar data value or a table data type.
Different Kinds of User-Defined Functions created are:
  * Scalar User-Defined Function: A Scalar user-defined function returns one of the scalar data types. Text, ntext, image and timestamp data types are not supported. These are the type of user-defined functions that most developers are used to in other programming languages. You pass in 0 to many parameters and you get a return value.
  * Inline Table-Value User-Defined Function: An Inline Table-Value user-defined function returns a table data type and is an exceptional alternative to a view as the user-defined function can pass parameters into a T-SQL select command and in essence provide us with a parameterized, non-updateable view of the underlying tables.
  * Multi-statement Table-Value User-Defined Function: A Multi-Statement Table-Value user-defined function returns a table and is also an exceptional alternative to a view as the function can support multiple T-SQL statements to build the final result where the view is limited to a single SELECT statement. Also, the ability to pass parameters into a TSQL select command or a group of them gives us the capability to in essence create a parameterized, non-updateable view of the data in the underlying tables. Within the create function command you must define the table structure that is being returned. After creating this type of user-defined function, It can be used in the FROM clause of a T-SQL command unlike the behavior found when using a stored procedure which can also return record sets.

* <b>What is Identity? </b></br>

  Identity (or AutoNumber) is a column that automatically generates numeric values. A start and increment value can be set, but most DBA leave these at 1. A GUID column also generates numbers; the value of this cannot be controlled. Identity/GUID columns do not need to be indexed.

* <b>What is Data Warehousing?</b></br>
  * Subject-oriented, meaning that the data in the database is organized so that all the data elements relating to the same real-world event or object are linked together;
  * Time-variant, meaning that the changes to the data in the database are tracked and recorded so that reports can be produced showing changes over time;
  * Non-volatile, meaning that data in the database is never over-written or deleted, once committed, the data is static, read-only, but retained for future reporting.
  * Integrated, meaning that the database contains data from most or all of an organization's operational applications, and that this data is made consistent.

* <b>What is the difference between SQL and MySQL or SQL Server?</b></br>

  SQL or Structured Query Language is a language; language that communicates with a relational database thus providing ways of manipulating and creating databases. MySQL and Microsoft’s SQL Server both are relational database management systems that use SQL as their standard relational database language.

* <b>What is the difference between SQL and PL/SQL?</b></br>

  SQL or Structured Query Language is a language which is used to communicate with a relational database. It provides a way to manipulate and create databases. On the other hand, PL/SQL is a dialect of SQL that adds procedural features of programming languages in SQL. It was developed by Oracle Corporation in the early 90's to enhance the capabilities of SQL.</br>
  Read more: [GeeksforGeeks](https://www.geeksforgeeks.org/sql-interview-questions/)

* <b>What are various DDL commands in SQL? Give brief description of their purposes.</b></br>

  Following are various DDL or Data Definition Language commands in SQL −

  * CREATE − it creates a new table, a view of a table, or other object in database.
  * ALTER − it modifies an existing database object, such as a table.
  * DROP − it deletes an entire table, a view of a table or other object in the database.

* <b>What are various DML commands in SQL? Give brief description of their purposes.</b></br>

  Following are various DML or Data Manipulation Language commands in SQL −

  * SELECT − it retrieves certain records from one or more tables.
  * INSERT − it creates a record.
  * UPDATE − it modifies records.
  * DELETE − it deletes records.

* <b>What are various DCL commands in SQL? Give brief description of their purposes.</b></br>

  Following are various DCL or Data Control Language commands in SQL −

 * GRANT − it gives a privilege to user.
 * REVOKE − it takes back privileges granted from user.

* <b>Can you sort a column using a column alias?</b></br>

  Yes. A column alias could be used in the ORDER BY clause.

* <b>What is Transaction Control Language (TCL)?</b></br>

  TCL is a category of SQL commands which primarily deals with the database transaction and save points. These keywords implement the SQL functions and logic defined by the developer into the database structure and behavior. Examples of these TCL commands are:

  * COMMIT – used to commit a transaction
  * ROLLBACK – in any advent of errors, transaction rollback is invoked by this keyword.
  * SAVEPOINT – keyword representing the reverting point of rollback
  * SET TRANSACTION – sets the specifics of the transaction

* <b>Is a NULL value same as zero or a blank space? If not then what is the difference?</b></br>

  A NULL value is not same as zero or a blank space. A NULL value is a value which is ‘unavailable, unassigned, unknown or not applicable’. Whereas, zero is a number and blank space is a character.

* <b>If a table contains duplicate rows, does a query result display the duplicate values by default? How can you eliminate duplicate rows from a query result?</b></br>

 A query result displays all rows including the duplicate rows. To eliminate duplicate rows in the result, the DISTINCT keyword is used in the SELECT clause.

* <b>How do you search for a value in a database table when you don’t have the exact value to search for?</b></br>

  In such cases, the LIKE condition operator is used to select rows that match a character pattern. This is also called ‘wildcard’ search.

* <b>What is the default ordering of data using the ORDER BY clause? How could it be changed?</b></br>

  The default sorting order is ascending. It can be changed using the DESC keyword, after the column name in the ORDER BY clause.

* <b>What are the specific uses of SQL functions?</b></br>

  SQL functions have the following uses −

  * Performing calculations on data
  * Modifying individual data items
  * Manipulating the output
  * Formatting dates and numbers
  * Converting data types

* <b>What are the case manipulation functions of SQL?</b></br>

  There are three types of case manipulation functions available in SQL. They are,
  * LOWER: The purpose of this function is to return the string in lowercase. It takes a string as argument and returns the string by converting it into lower case.
  Syntax:</br>
  `LOWER('string')`</br>

  * UPPER:The purpose of this function is to return the string in uppercase. It takes a string as argument and returns the string by converting it into uppercase.
  Syntax:</br>
  `UPPER('string')`</br>
  * INITCAP:The purpose of this function is to return the string with first letter in uppercase and rest of the letters in lowercase.
  Syntax:
  `INITCAP('string')`

* <b>What is the use of the NULLIF function?</b></br>

  The NULLIF function compares two expressions. If they are equal, the function returns null. If they are not equal, the first expression is returned.

* <b>Discuss the syntax and use of the COALESCE function?</b></br>

  The COALESCE function has the expression COALESCE(exp1, exp2, …. expn)

  It returns the first non-null expression given in the parameter list.

* <b>Which expressions or functions allow you to implement conditional processing in a SQL statement?</b></br>

  There are two ways to implement conditional processing or IF-THEN-ELSE logic in a SQL statement.

  * Using CASE expression
  * Using the DECODE function

* <b>You want to display a result query from joining two tables with 20 and 10 rows respectively. Erroneously you forget to write the WHERE clause. What would be the result?</b></br>

  The result would be the Cartesian product of two tables with 20 x 10 = 200 rows.

* <b>What is the difference between cross joins and natural joins?</b></br>

  The cross join produces the cross product or Cartesian product of two tables. The natural join is based on all the columns having same name and data types in both the tables.

* <b>What is the purpose of the group functions in SQL? Give some examples of group functions.</b></br>

  Group functions in SQL work on sets of rows and returns one result per group. Examples of group functions are AVG, COUNT, MAX, MIN, STDDEV, SUM, VARIANCE.

* <b>What’s wrong in the following query?
  ```SQL
   SELECT subject_code, AVG (marks)
   FROM students
   WHERE AVG(marks) > 75
   GROUP BY subject_code;
   ```
   </b></br>
   The WHERE clause cannot be used to restrict groups. The HAVING clause should be used.
  ```SQL
     SELECT subject_code, AVG (marks)
     FROM students
     HAVING AVG(marks) > 75
     GROUP BY subject_code;
     ```
* <b>Say True or False. Give explanation if False.

  Group functions cannot be nested.</b></br>
  False. Group functions can be nested to a depth of two.

* <b>How do you insert null values in a column while inserting data?</b></br>

  Null values can be inserted into a table by one of the following ways −

  * Implicitly by omitting the column from the column list.
  * Explicitly by specifying the NULL keyword in the VALUES clause.

* <b>What happens if you omit the WHERE clause in the UPDATE statement?</b></br>

  All the rows in the table are modified.

* <b>Can you modify the rows in a table based on values from another table? Explain.</b></br>

  Yes. Use of subqueries in UPDATE statements allow you to update rows in a table based on values from another table.

* <b>What happens if you omit the WHERE clause in a delete statement?</b></br>

  All the rows in the table are deleted.

* <b>Can you remove rows from a table based on values from another table? Explain.</b></br>

  Yes, subqueries can be used to remove rows from a table based on values from another table.

* <b>What is the purpose of the MERGE statement in SQL?</b></br>

  The MERGE statement allows conditional update or insertion of data into a database table. It performs an UPDATE if the rows exists, or an INSERT if the row does not exist.

* <b>Which SQL statement is used to add, modify or drop columns in a database table?</b></br>

  The ALTER TABLE statement.

* <b>What are Constraints in SQL?</b></br>

  Constraints are used to specify the rules concerning data in the table. It can be applied for single or multiple fields in an SQL table during creation of table or after creationg using the ALTER TABLE command. The constraints are:

    * NOT NULL - Restricts NULL value from being inserted into a column.
    * CHECK - Verifies that all values in a field satisfy a condition.
    * DEFAULT - Automatically assigns a default value if no value has been specified for the field.
    * UNIQUE - Ensures unique values to be inserted into the field.
    * INDEX - Indexes a field providing faster retrieval of records.
    * PRIMARY KEY - Uniquely identifies each record in a table.
    * FOREIGN KEY - Ensures referential integrity for a record in another table.

* <b>What are UNION, MINUS and INTERSECT command</b></br>

  * The UNION operator combines and returns the result-set retrieved by two or more SELECT statements.
  * The MINUS operator in SQL is used to remove duplicates from the result-set obtained by the second SELECT query from the result-set obtained by the first SELECT query and then return the filtered results from the first.
  * The INTERSECT clause in SQL combines the result-set fetched by the two SELECT statements where records from one match the other and then returns this intersection of result-sets.

  Certain conditions need to be met before executing either of the above statements in SQL -

  * Each SELECT statement within the clause must have the same number of columns
  * The columns must also have similar data types
  * The columns in each SELECT statement should necessarily have the same order

* <b>What are Entities and Relationships?</b></br>

  Entity: An entity can be a real-world object, either tangible or intangible, that can be easily identifiable. For example, in a college database, students, professors, workers, departments, and projects can be referred to as entities. Each entity has some associated properties that provide it an identity.

  Relationships: Relations or links between entities that have something to do with each other. For example - The employees table in a company's database can be associated with the salary table in the same database.

* <b>List the different types of relationships in SQL.</b></br>

  * One-to-One - This can be defined as the relationship between two tables where each record in one table is associated with the maximum of one record in the other table.
  * One-to-Many & Many-to-One - This is the most commonly used relationship where a record in a table is associated with multiple records in the other table.
  * Many-to-Many - This is used in cases when multiple instances on both sides are needed for defining a relationship.
  * Self Referencing Relationships - This is used when a table needs to define a relationship with itself.

* <b>What is an Alias in SQL?</b></br>

  An alias is a feature of SQL that is supported by most, if not all, RDBMSs. It is a temporary name assigned to the table or table column for the purpose of a particular SQL query. In addition, aliasing can be employed as an obfuscation technique to secure the real names of database fields. A table alias is also called a correlation name .

  An alias is represented explicitly by the AS keyword but in some cases the same can be performed without it as well. Nevertheless, using the AS keyword is always a good practice.

* <b>What are Aggregate and Scalar functions?</b></br>

  An aggregate function performs operations on a collection of values to return a single scalar value. Aggregate functions are often used with the GROUP BY and HAVING clauses of the SELECT statement. Following are the widely used SQL aggregate functions:

  * AVG() - Calculates the mean of a collection of values.
  * COUNT() - Counts the total number of records in a specific table or view.
  * MIN() - Calculates the minimum of a collection of values.
  * MAX() - Calculates the maximum of a collection of values.
  * SUM() - Calculates the sum of a collection of values.
  * FIRST() - Fetches the first element in a collection of values.
  * LAST() - Fetches the last element in a collection of values.
  Note: All aggregate functions described above ignore NULL values except for the COUNT function.

  A scalar function returns a single value based on the input value. Following are the widely used SQL scalar functions:

  * LEN() - Calculates the total length of the given field (column).
  * UCASE() - Converts a collection of string values to uppercase characters.
  * LCASE() - Converts a collection of string values to lowercase characters.
  * MID() - Extracts substrings from a collection of string values in a table.
  * CONCAT() - Concatenates two or more strings.
  * RAND() - Generates a random collection of numbers of given length.
  * ROUND() - Calculates the round off integer value for a numeric field (or decimal point values).
  * NOW() - Returns the current data & time.
  * FORMAT() - Sets the format to display a collection of values.

* <b>What is a Stored Procedure?</b></br>

  A stored procedure is a subroutine available to applications that access a relational database management system (RDBMS). Such procedures are stored in the database data dictionary. The sole disadvantage of stored procedure is that it can be executed nowhere except in the database and occupies more memory in the database server. It also provides a sense of security and functionality as users who can't access the data directly can be granted access via stored procedures.

* <b>What is a Recursive Stored Procedure?</b></br>

  A stored procedure which calls itself until a boundary condition is reached, is called a recursive stored procedure. This recursive function helps the programmers to deploy the same set of code several times as and when required. Some SQL programming languages limit the recursion depth to prevent an infinite loop of procedure calls from causing a stack overflow, which slows down the system and may lead to system crashes.

* <b>How to create empty tables with the same structure as another table?</b></br>

  Creating empty tables with the same structure can be done smartly by fetching the records of one table into a new table using the INTO operator while fixing a WHERE clause to be false for all records. Hence, SQL prepares the new table with a duplicate structure to accept the fetched records but since no records get fetched due to the WHERE clause in action, nothing is inserted into the new table.

  ```SQL
  SELECT * INTO Students_copy
  FROM Students WHERE 1 = 2;
  ```
* <b>How can we link a SQL database to an existing Android App?</b></br>

  It will require a JDBC (Java Database Connectivity) driver to link these two. Also, you must add the corresponding dependencies to your build.gradle file along with the permissions and grants.

* <b>What are transaction and its controls?</b></br>

  A transaction can be defined as the sequence task that is performed on databases in a logical manner to gain certain results. Operations performed like Creating, updating, deleting records in the database comes from transactions.

  In simple word, we can say that a transaction means a group of SQL queries executed on database records.

  There are 4 transaction controls such as

  * COMMIT: It is used to save all changes made through the transaction
  * ROLLBACK: It is used to roll back the transaction such as all changes made by the transaction are reverted back and database remains as before
  * SET TRANSACTION: Set the name of transaction
  * SAVEPOINT: It is used to set the point from where the transaction is to be rolled back

* <b>Explain the working of SQL Privileges?</b></br>

  SQL GRANT and REVOKE commands are used to implement privileges in SQL multiple user environments.  The administrator of the database can grant or revoke privileges to or from users of database object like SELECT, INSERT, UPDATE, DELETE, ALL etc.

  * GRANT Command: This command is used provide database access to user apart from an administrator.
  ```SQL
  GRANT privilege_name
  ON object_name
  TO {user_name|PUBLIC|role_name}
  [WITH GRANT OPTION];
  ```
  In above syntax WITH GRANT OPTIONS indicates that the user can grant the access to another user too.

  * REVOKE Command: This command is used provide database deny or remove access to database objects.
  ```SQL
  REVOKE privilege_name
  ON object_name
  FROM {user_name|PUBLIC|role_name};
  ```

* <b>How many types of Privileges are available in SQL?</b></br>

  There are two types of privileges used in SQL, such as

  * System Privilege: System privileges deal with an object of a particular type and specifies the right to perform one or more actions on it which include Admin allows a user to perform administrative tasks, ALTER ANY INDEX, ALTER ANY CACHE GROUP CREATE/ALTER/DELETE TABLE, CREATE/ALTER/DELETE VIEW etc.
  * Object Privilege: This allows to perform actions on an object or object of another user(s) viz. table, view, indexes etc. Some of the object privileges are EXECUTE, INSERT, UPDATE, DELETE, SELECT, FLUSH, LOAD, INDEX, REFERENCES etc.

* <b>What is SQL Injection?</b></br>

  SQL Injection is a type of database attack technique where malicious SQL statements are inserted into an entry field of database such that once it is executed the database is opened for an attacker. This technique is usually used for attacking Data-Driven Applications to have an access to sensitive data and perform administrative tasks on databases.

  For Example: `SELECT column_name(s) FROM table_name WHERE condition;`

* <b>What is SQL Sandbox in SQL Server?</b></br>

  SQL Sandbox is the safe place in SQL Server Environment where untrusted scripts are executed. There are 3 types of SQL sandbox, such as

  * Safe Access Sandbox: Here a user can perform SQL operations such as creating stored procedures, triggers etc. but cannot have access to the memory and cannot create files.
  * External Access Sandbox: User can have access to files without having a right to manipulate the memory allocation.
  * Unsafe Access Sandbox: This contains untrusted codes where a user can have access to memory.

* <b>What is the Cartesian product of table?</b></br>

  The output of Cross Join is called as a Cartesian product. It returns rows combining each row from the first table with each row of the second table. For Example, if we join two tables having 15 and 20 columns the Cartesian product of two tables will be 15×20=300 Rows.

* <b>What is the difference between Nested Subquery and Correlated Subquery?</b></br>

  Subquery within another subquery is called as Nested Subquery.  If the output of a subquery is depending on column values of the parent query table then the query is called Correlated Subquery.

  `SELECT adminid(SELEC Firstname+' ‘+Lastname  FROM Employee WHERE
  empid=emp. adminid)AS EmpAdminId FROM Employee`

  This query gets details of an employee from the Employee table.

* <b> What do we need to check in Database Testing?</b></br>

  Generally, in Database Testing following thing is need to be tested

  * Database Connectivity
  * Constraint Check
  * Required Application Field and its size
  * Data Retrieval and Processing With DML operations
  * Stored Procedures
  * Functional flow

* <b>What is Database White Box Testing?</b></br>

  Database White Box Testing involves

  * Database Consistency and ACID properties
  * Database triggers and logical views
  * Decision Coverage, Condition Coverage, and Statement Coverage
  * Database Tables, Data Model, and Database Schema
  * Referential integrity rules

* <b>What is Database Black Box Testing?</b></br>

  Database Black Box Testing involves

  * Data Mapping
  * Data stored and retrieved
  * Use of Black Box techniques such as Equivalence Partitioning and Boundary Value Analysis (BVA)

* <b>What is identity in SQL?</b></br>

  An identity column in the SQL automatically generates numeric values. We can define a start and increment value of the identity column.

* <b>What do you mean by ROWID?</b></br>

  It’s an 18 character long pseudo column attached with each row of a table.

* <b>What is Case Function?</b></br>

  Case facilitates if-then-else type of logic in SQL. It evaluates a list of conditions and returns one of the multiple possible result expressions.

* <b>Define a temp table.</b></br>

  A temp table is a temporary storage structure to store the data temporarily.

* <b>Explain the difference between Rename and Alias?</b></br>

  Rename is a permanent name given to a table or column whereas Alias is a temporary name given to a table or column.

* <b> What are the advantages of Views?</b></br>

  Advantages of Views:

  * Views restrict access to the data because the view can display selective columns from the table.
  * Views can be used to make simple queries to retrieve the results of complicated queries. For example, views can be used to query information from multiple tables without the user knowing.

* <b>Can a View based on another View?</b></br>

  Yes, A View is based on another View.

* <b>What is the difference between Local and Global temporary table?</b></br>

  If defined in inside a compound statement a local temporary table exists only for the duration of that statement but a global temporary table exists permanently in the DB but its rows disappear when the connection is closed.

* <b>What is CTE?</b></br>

  A CTE or common table expression is an expression which contains temporary result set which is defined in a SQL statement.

* <b>Read More:</b></br>

  * [10 Frequently asked SQL Query Interview Questions](http://java67.blogspot.com.by/2013/04/10-frequently-asked-sql-query-interview-questions-answers-database.html)
  * [45 Essential SQL Interview Questions from Toptal](http://www.toptal.com/sql/interview-questions) (Must Read)
  * [Common Interview Questions and Answers](http://www.indiabix.com/technical/sql-server-common-questions/)
  * [General Interview Questions and Answers](http://www.indiabix.com/technical/sql-server-general-questions/)
  * [Schema, Questions & Solutions for SQL Exercising](https://github.com/XD-DENG/SQL-exercise) (Must Read)
  * [SQL Interview Questions that have been designed specially to get you acquainted with the nature of questions you may encounter during your interview for the subject of SQL](http://www.tutorialspoint.com/sql/sql_interview_questions.htm) (Must Read for TRUE-FALSE Questions)
  * [SQL Interview Questions CHEAT SHEET](https://www.interviewbit.com/sql-interview-questions/) (Must Read)
  * [SQL Journaldev Questions](https://www.journaldev.com/17773/sql-interview-questions-answers)
  * [SQL 50 Popular SQL Interview Questions for Testers](https://www.softwaretestinghelp.com/50-popular-sql-interview-questions-for-testers/)
  * [GeeksforGeeks SQL Interview Questions](https://www.geeksforgeeks.org/sql-interview-questions/)
  * [50 SQL Query Questions and Answers for Practice](https://www.techbeamers.com/sql-query-questions-answers-for-practice/) (Must Read)
  * [SQL Queries for Interview](https://artoftesting.com/interviewSection/sql-queries-for-interview.html) (Must Read)
  * Jitbit's SQL interview questions [GitHub Gist](https://gist.github.com/mjhea0/5667162)

### SQLite

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
