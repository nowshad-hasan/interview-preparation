Collections - 
- [InterviewBit](https://www.interviewbit.com/hibernate-interview-questions/)
- [InterviewBit JPA](https://www.interviewbit.com/jpa-interview-questions/)
- [indeed](https://in.indeed.com/career-advice/interviewing/spring-jpa-interview-questions)
- [geeksforgeeks](https://www.geeksforgeeks.org/advance-java/hibernate-interview-questions/)
- [flexipie](https://flexiple.com/jpa/interview-questions)
- [Simple learn](https://www.simplilearn.com/hibernate-interview-questions-article)
- [digitalocean](https://www.digitalocean.com/community/tutorials/hibernate-interview-questions-and-answers#hibernate-tools-eclipse-plugin)
- [java revisited](https://javarevisited.blogspot.com/2013/05/10-hibernate-interview-questions-answers-java-j2ee-senior.html)
- [Medium](https://medium.com/@pratik.941/important-jpa-interview-questions-a-detailed-guide-5c1405e0927b)

Questions - 

- **JPA Vs Spring Data JPA Vs Hibernate**

- **What are the advantages of Hibernate over JDBC?**
  - Clean Readable Code - We can eliminate JDBC API based boiler plate codes using cleaner code.
  - HQL (Hibernate Query Language) - It provides HQL which is like object oriented nature. So, we don't need to write raw queries and when we write HQL (or JPQL) we write this database independently.But in JDBC, we need to write queries for that database explicitly.
  - Transaction management - JDBC does not support implicit transaction management. We need to write the transaction code ourselves. But for hibernate, it implicitly gives the feature.
  - Exception handling - If we write JDBC code, we need to wrap the code with `try/catch` as SQLException is a checked exception. But with hibernate, it wraps the JDBC exceptions with unchecked exception like JDBCException or HibernateException. So, as a developer our code is clean as we can avoid multiple try-catch block.
  - OOP - Hibernate supports OOPs features like inheritance, associations, and collections. But JDBC does not support any of these.

- **What is ORM in Hibernate?**
  - ORM stands for Object Relational Mapping. This is a mapping tool pattern where data stored in relational database to an object used in object-oriented programming. This tool also helps greatly in simplifying data retrieval, creation and manipulation. 

- **Is hibernate prone to SQL injection attack?**
  - No, hibernate is not immune to SQL injection. Buty following good practices can avoid SQL injection attack.
    - Incorporate Prepared Statements that use parameterised queries.
    - Ensure data sanity by doing input validation.

- **Can you explain the concept behind Hibernate Inheritance Mapping?**
  - This concept means that how hibernate as an ORM tries to map the inheritance of Java and flat structure of Databases. There are 4 different inheritance mapping strategies available:
    - Single Table
    - Table Per Class
    - Mapped Super Class
    - Joined Table

- **How do you create an immutable class in hibernate?**
  - We can use @Immutable annotation.
  
- **What can you tell about Hibernate Configuration File??**
  - The name of the configuration file is `hibernate.cfg.xml` or `hibernate.properties`. It is one of most required files in Hibernate. By default, this file is placed under the `src/main/resource` folder. It contains below information - 
    - Database connection details - Driver class, URL, username, password
    - If we want to connect two database, we need two configurations files with different names
    - Hibernate properties - Dialect, show_sql, second_level_cache and mapping file names

- **what is lazy loading in hibernate?**
  - It improves application performance by helping to load child objects on demand. That means, child objects are not loaded if parent is not loaded.

- **What is a SessionFactory?**
  - SessionFactory gives the Session object. This Session object is used to establish the database connection. As a good practice, the application generally has a single instance of SessionFactory.

- **What is a Session in Hibernate?**
  - A session is an object that maintains the connection between the Java application and the database. It has methods for storing, retrieving, modifying or deleting data from database using methods like persist(), load(), update(), delete() etc. Again, it has factory methods to return Query, Criteria, and Transaction objects.

- **What is the Hibernate caching?**
  -  Hibernate caching is a strategy for application performance by pooling objects in the cache so that the queries are executed faster. It is particularly helpful when fetching the same data multiple times. So, we will not hit the database everytime but access the data from the cache. 

- **What is the difference between first level cache and second level cache?** 
  - First level cache:
    - It is enabled by default. 
    - It belongs to hibernate session object
    - As it belongs to session object, so the data stored in one session will not be available in other session. So, the cached object will not be available to the whole application as application can use multiple session objects. 
  - Second level cache:
    - This is not available by default. We need to enable this explicitly.
    - As it belongs to SessionFactory object, the cached data is accessible by the entire application.
    - EH(Easy Hibernate) cache, Swarm cache, OS cache, JBoss cache are some example of cache providers.

- **What will happen if we call get() method in terms of cache?**
  - If any entity or object is loaded by `get()` method, the Hibernate will check the first level cache. Then it goes to second level cache if configured. If still not found, then it goes to the database and returns the object. If the row does not exist, then it returns null.

- **What are the main elements of Hibernate?** 
  - SessionFactory - This gives us a factory method to get session objects and clients of ConnectionProvider. It holds second-level-cache if configured.
  - Session - This is a short lived object that acts as an interface between the java application objects and database data. It is used to generate transaction, query and criteria objects. It holds first-level-cache by-default. 
  - Transaction - This object specifies the atomic unit of work which has some methods for transaction management. 
  - TransactionFactory - This is a factory of transaction objects. 
  - ConnectionProvider - This is a factory of JDBC connection objects and it provides an abstraction to the application from the DriverManager.

- **Can you tell the difference between getCurrentSession and openSession methods?**
  - getCurrentSession - This method returns the session bound to the context. This session object gets closed once the session factory is closed. In a single-threaded environment, this method is faster than openSession().
  - openSession - This method always opens a new session. And in a multi-threaded environment, for each request a new session object will be created. And for that we don't need to configure anything. But, as a developer we need to close this object after all database operations are done. And in single threaded environment, it is slower than getCurrentSession().

- **Differentiate between save() and saveOrUpdate() methods in hibernate session.**
  - Save - it generates a new identifier and INSERT new record in the database. So, the insertion fails if the primary key already exists in the table. The return type is Serializable which is the newly generated identifier id value as a Serializable object. It takes only transient (new) object to a persistent state.
  - saveOrUpdate - It can either INSERT or UPDATE based on existence of a record. If the primary key exists, the record is updated. And the return is void for this method. This method takes both transient (new) and detached (existing) objects into a persistent state. It is often used to re-attach a detached object into a session.
  - Note - So, saveOrUpdate() is more flexible in terms of use but it has overhead for extra processing to find out whether a record already exists in database or not.

- **Differentiate between get() and load() in Hibernate session**
  - get - This method gets the data from the database directly when it is called. That means, everytime it is called, it hits the database. If object is not found, it returns `null`. It should be used when we are unsure about the existence of data in the database.
  - load - This method returns a proxy object and loads the data only when it is actually required. It is `lazy loading` and it hits the database when it is actually required. If object is not found, it throws `ObjectNotFoundException`. This method should be used only when the data is present in the database. 

- **What is criteria API in hibernate?**
  - This API helps developers to build dynamic criteria queries on database. It is more powerful than HQL for creating dynamic queries. It helps us to build queries programmatically.
  
- **What is HQL?**
  - Hibernate Query Language (HQL) is used as an extension of SQL. It has some beautiful, widely used interfaces that helps us to perform complex queries very easily. 

- **What are Many to Many associations?**
  - This association indicates that there are multiple relations between the instances of two entities. This relationship creates a separate table to hold the foreign keys. And this third table is called `Join Table`.

- **What does session.lock() method in hibernate do?**
  - session.lock() method is used to reattach a detached object to the session.

- **When is merge() method of the hibernate session useful?**
  - This method is used for updating existing values. But the special feature is - after value update, it gives a copy of that object to persistent context and tracked for any changes. Before calling the `merge` method, the object was not initially tracked. 

- **Can you tell the difference between setMaxResults() and setFetchSize() of Query?**
  - setMaxResults - This function works similar to LIMIT/TOP in SQL. It is implemented by all database drivers.
  - setFetchSize - It works for optimizing how Hibernate sends the result to the caller, like - how the results are buffered, are they sent in different size chunks etc. It controls how efficiently data is transferred. It improve performance for large queries. In summary, it is used to optimize performance when retrieving a large number of rows. It is not implemented by all database drivers. 

- **Does Hibernate support Native SQL Queries?**
  - Of course. It provides the `createSQLQuery` method to run a raw query. Here is an example below.
  ```java
    Query query = session.createSQLQuery( "select * from employee ibe where ibe.fullName = :fullName")
                   .addEntity(Employee.class)
                   .setParameter("fullName", "Hibernate"); //named parameters
    List result = query.list();
    ```
- **Can we declare the Entity class final?**    
  - We should not. Because, hibernate uses proxy classes and objects for lazy loading. It is achieved by extending the entity bean. If the entity class is made final, then it cannot be extended and so lazy loading can not be supported.

- **What are the states of a persistent entity?**
  - Transient:
    - This state is the initial state of any entity object. When any entity object is created it enters into this state.
    - In this state, the object is not linked to any session. So, it is not connected to any database table. That is why any changes to the object won't reflect to the database.
  
  - Persistent:
    - This state is entered when the object is linked to any session.
    - An object is said to be in a persistent state whenever we save or persist an object in the database. Each object corresponds to the row of the database table. So, any change to the object will reflect to the row of the database.
  
  - Detached:
    - The object enters into this state when the session is closed or the cache is cleared. 
    - Due to the object being no longer part of the session, any changes to this object will not reflect in the row of the database. However, it has still representation of the row of the database.
    - If we want to persist the changes of this object, it has to be reattached to the hibernate session. To do that we can use load(), merge(), refresh(), update() or save() on a new session reference to the detached object.

- **What is Query Cache?**
  - When any query with same parameter is frequently used, this query cache is useful. Additional configurations have to be done to enable this. Query cache is connected to second-level cache. 

- **Can you tell something about the N+1 SELECT problem in Hibernate?**
  - 