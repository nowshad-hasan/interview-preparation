### Spring core

- Two ways to configure ApplicationContext
- Component vs Bean
- All the common annotations - Controller, Component, Service, Repository
- Inversion Of Control (IOC)
- PreDestroy, PostConstruct
- Autowired
- Context, ApplicationContext
- BeanFactory vs ApplicationContext
- Constructor Injection over Field Injection:
- Qualifier
- What is @ComponentScan? Why we don't need to use @ComponentScan in Spring  Boot? 
- OpenSession Vs BeginSession
- Flush
- @Proxy, @Async
- HikariCP, Tomcat
- Bean Scopes
- How to inject Prototype Bean in Singleton Bean
- Transaction and its Isolation modes
- Servlet, Dispatcher servlet and ViewResolver
- RequestParam Vs PathVariable
- Different types of injection - method injection, property injection, constructor injection
- @Value

### Spring AOP

- Where we can apply AOP
- AOP uses in spring universe
- How to write an Aspect
- How AOP works with DynamicProxy design pattern
- JDK proxy vs CGLIB proxy
- What is PointCut, Advice, JointPoint
- Annotation used in AOP - Before, After

### Hibernate & JPA

- EntityManager vs Session
- What is Hibernate
- What is ORM and problems without ORM
- JPA vs Hibernate
- SessionFactory
- HBM2DDL command in config file
- @Entity Vs @Table
- Transient
- @Basic, @LOB, @CLOB, @BLOB
- PrimaryKey vs SurrogateKey
- @GeneratedValue
- Embedded Object: @Embeddable
- Embeded Collection
- @JoinTable, @JoinColumn
- @CollectionId
- Hibernate Proxy Object for Session.get()
- OneToOne, OneToMany, ManyToOne, ManyToMany. And their fetch default operation.
- Hibernate Collections
- Cascade
- Inheritance
- Transient vs Persistent Vs Detached Objects. And their state changing behaviour.
- HQL, JPQL
- Criteria API
- Cache - first level cache, second level cache, Query Cache
- Save vs Persist
- Hibernate N+1 Problem
- Optimistic vs Pessimistic locking

### Spring Security

- Encode vs Encrypt
- Authentication vs Authorization
- Principal, Authority, Role
- Filter
- SecurityContext
- The spring security full diagram
- AuthenticationManage, AuthenticationProvider
- User, UserDetailsService
- CORS, CSRF. How CSRF enabled by default? How it works with Spring Security?
- Structure of JWT
- Password Encoder
- MvcMatchers vs AntMatchers
- What is LDAP