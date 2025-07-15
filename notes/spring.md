Collections - 
 - [Baeldung](https://www.baeldung.com/spring-boot-interview-questions)
 - [Medium 1](https://medium.com/@sharmapraveen91/30-advanced-spring-boot-interview-questions-for-experienced-professionals-3574173472c1)
 - [Medium 2](https://codefarm0.medium.com/300-spring-boot-interview-questions-43393e1c2bef)
 - [InterviewBit](https://www.interviewbit.com/spring-boot-interview-questions/)
 - [simple learn](https://www.simplilearn.com/spring-boot-interview-questions-article)
 - [geeksforgeeks](https://www.geeksforgeeks.org/springboot/spring-boot-interview-questions-and-answers/)
 - [Java Techie 1](https://youtu.be/fWHo7RDUMhA?si=lBPW57RZm-Zdsttz)
 - [Java Techie 2](https://youtu.be/-_tPeb3VE6w?si=2jQrjNloDTIU89Tf)
 - [Youtube](https://youtu.be/vp1m6YGKo9A?si=b0uIiGNvPDIbM7PS)
 - [GenZ Career 1](https://www.youtube.com/watch?v=XilRv9wJhzc&ab_channel=GenZCareer)
 - [GenZ Career 2](https://www.youtube.com/watch?v=gSwgHC5apX8&ab_channel=GenZCareer)
 - [Learn code with Durgesh](https://youtu.be/5wzEz_eNJMw?si=mNsGEy5SseUUVl7G)
 - [in28Minutes](https://github.com/in28minutes/spring-interview-guide)

Questions:

- **What is the difference between Spring and Spring Boot?**

- **How do you optimize the startup time of a Spring Boot application in a production environment?**
  - Lazy initialization - We can use `spring.main.lazy-initialization=true` to delay bean initialization until needed.
  - Profile specific configuration - We can separate different profiles for different environments to avoid unnecessary loading.
  - Component scanning - We can restrict component scanning using `@ComponentScan` to only include essential packages.
  - Reduce bean creation - We can avoid unnecessary beans during startup, especially for time-sensitive services.

- **Explain the concept of Spring Boot’s @ConfigurationProperties with complex objects. How would you handle nested configurations?**
  - This annotation helps us to map configuration files into java object. Yes we could do this with `@Value`, but that code will be repetitive. And this way is better when working with complex properties file. Here is an example.
  
  ```java
    @Component
    @ConfigurationProperties(prefix = "app")
    public class AppProperties {
        private String name;
        private Database database;

        public static class Database {
            private String url;
            private String username;
            private String password;
            // getters and setters
        }

        // getters and setters
    }
  ```

  For the config file - 

  ```yaml
    app:
        name: MyApp
        database:
            url: jdbc:mysql://localhost:3306/mydb
            username: root
            password: secret
  ```
- **What are the main challenges with distributed tracing in Spring Boot microservices, and how do you implement it?**
  - Distributed tracing helps us to track requests across multiple microservices. The main challenges are - latency, proper correlation of requests, aggregating result across the services. The solutions are - 
    - Spring Cloud Sleuth:  Automatically instruments Spring Boot applications for distributed tracing.
    - Integration with Zipkin or Jaeger: Use Sleuth with tools like Zipkin for trace visualization and monitoring.
    - Correlation: Propagate TraceId and SpanId headers for cross-service correlation, ensuring traceability.
  - By implementing distributed tracing we gain better visibility in service communication and identify service bottlenecks.   

- **How would you implement a robust custom health check in Spring Boot for a production environment?**
  - `Actuator` allows creating custom-health-monitoring for production environment. Implementing a custom `HealthIndicator` ensures that we can check specific resources like, database, external system, file system etc.
  
  ```java
    @Component
    public class MyCustomHealthIndicator extends AbstractHealthIndicator {
        @Override
        protected void doHealthCheck(Health.Builder builder) throws Exception {
            boolean isHealthy = checkDatabaseConnection();
            if (isHealthy) {
                builder.up().withDetail("Database", "Available");
            } else {
                builder.down().withDetail("Database", "Not Available");
            }
        }
    }
  ```

-  **How do you handle service discovery in a Spring Boot microservices architecture?**
   -  Spring Cloud's `Eureka` is widely used for dynamic service registration and discovery. We can enable `@EnableEurekaClient` to register services with Eureka. 

- **What is Spring Boot’s @Retryable annotation, and how do you fine-tune it for microservices reliability?**
  - The @Retryable annotation allows retrying a method call in case of failure. This is essential when any service that might experience transient failures (e.g., network timeouts or database issues).
  
  ```java
    @Retryable(value = {IOException.class}, maxAttempts = 5, backoff = @Backoff(delay = 2000))
    public String fetchData() {
        // API call that might fail
    }
  ```

- **How can you implement and manage custom security policies in Spring Boot for fine-grained access control?**
  - Spring boot has multiple annotations, like - `@PreAuthorize`, `@Secured`, `@RolesAllowed` to secure methods.    
  
  ```java
    @PreAuthorize("hasRole('ADMIN')")
    public String performAdminTask() {
        return "Admin Task Completed";
    }
  ```
- **How do you handle versioning in Spring Boot APIs?**
  - API versioning is crucial for maintaining backward compatibility when our application grows. There are few ways below - 
    - URL versioning: `/api/v1/resource`
    - Parameter versioning: `/api/resource?version=1`
    - Header-based versioning:  Using custom header `API-Version`

- **How do you implement multi-tenancy in Spring Boot applications?**
  - Multi-tenancy allows a single instance of an application to server multiple tenants each with its own data. We can achieve this with separate ways. 
    - Database per tenant: Use dynamic routing to select the correct database based on tenant information. 
    - Schema per tenant: Use single database but separate schema for each tenant
  - We can implement this by changing data source or schema based on tenant context, typically extracted from the HTTP request headers or authentication token.

- **How do you manage external configurations in a Spring Boot application across multiple environments?**
  - Spring Boot allows to manage external configurations with:
    - Profile: Use `@Profile` to define beans for specific environments, like - `@Profile("prod")`.
    - application.properties or yaml: Use `application-prod.properties` for production-specific configurations. 
    - Spring cloud config: For distributed system, we can use Spring Cloud Config Server to manage configurations centrally. 

- **What are some strategies for debugging a Spring Boot application in production?**
  - Spring Boot Actuator: It provides insights into health, metrics and environment information.
  - Logging: We can use `SLF4J` or `Logback` for better traceability.
  - Remote debugging: Enable remote debugginh via the JVM by passing `-agentlib:jdwp` parameters. 
  - Heap Dumps & Thread Dumps: We can capture heap dumps and thread dumps during application issues. 

- **How would you implement Spring Boot Security with OAuth 2.0 for a microservices-based system?**
  - OAuth 2.0 provides authorization by issuing access tokens. For spring boot, we can use `Spring Security OAuth2` for managing authentication. 
    - OAuth2 Authorization Server - Use Spring Security OAuth to configure an OAuth2 Authorization Server for issuing tokens.
    - OAuth2 Resource Server: Use @EnableResourceServer to secure resources by validating incoming OAuth2 tokens.

- **What are some common performance bottlenecks in Spring Boot applications and how do you resolve them?**
  - Database access: Optimize queries, add index properly, use pagination and consider connection pooling (e.g. - HikariCP).
  - Memory leaks: Use tools like `VisualVM` to monitor memory usage to avoid memory leaks. 
  - Thread Pooling: We can properly size thread pools for handling HTTP requests and background tasks. 
  - Caching: We can use Spring's caching abstraction (@Cacheable) to reduce the load on database.
  - Compress the response: We can add gzip compression configuration in properties file. It will compress every response by 70-90%. It works with JSON, HTML or text-based response. But it won't work with already compressed files like `.jpg`, `.png` or `.mp4` files. But it will cost CPU performance trying to compress it. This compression strategy helps us to work with low-bandwidth. In that case, it gives us faster network transfers.  

- **How do you handle asynchronous processing in Spring Boot?**
  - @Async Annotation: It is used for executing methods asynchronously.
  - Executor - Use Executor beans to control the threading model for asynchronous tasks.
  
  ```java
    @Async
    public CompletableFuture<String> processAsyncTask() {
        // Long-running task
        return CompletableFuture.completedFuture("Task completed");
    }
  ```

- **How would you implement caching in a Spring Boot application?**
  - At first we need to add `@EnableCaching` annotation in the main application. 
  
  ```java
    @SpringBootApplication
    @EnableCaching
    public class MyApplication {
        public static void main(String[] args) {
            SpringApplication.run(MyApplication.class, args);
        }
    }
    ```
   - Now we add `@Cacheable`  in any method to cache the result. Like below where if the `users` cache contains the value for the id, this method won't execute, it won't go to the database but return the result from the cache.
  
  ```java
    @Cacheable("users")
    public User getUserById(Long id) {
        System.out.println("Fetching from DB...");
        return userRepository.findById(id).orElse(null);
    }
  ```
  - But we need to update cache when result is changed otherwise we will get `stale` data. To update, we use `@CachePut` annotation. And this method always executes and updates the cache.
  
  ```java
    @CachePut(value = "users", key = "#user.id")
    public User updateUser(User user) {
        return userRepository.save(user);
    }
  ```
  - If we want to remove from the cache we use `@CacheEvict`.
  
  ```java
    @CacheEvict(value = "users", key = "#id")
    public void deleteUser(Long id) {
        userRepository.deleteById(id);
    }
  ```
  - But we need to remember something about caching. Like - we should not cache everything but only costly and stable data. And we should take care about memory limits. We should also add logging to observe cache hit/miss. And most importantly, we should use eviction or TTL properly.

- **How do you configure and manage Spring Boot logging in production?**
  - Logback: we can use default logging framework and use `logback-spring.xml` for configuration.
  - External Logging: Integrate with logging solutions like ELK (Elasticsearch, Logstash, Kibana) for centralizing logs.
  - Log levels: We can set different log levels per environment, like `INFO` for production, `DEBUG` for development.

- **How would you implement API Gateway using Spring Cloud Gateway in a Spring Boot-based microservices architecture?**
  - Spring Cloud Gateway is used for various purposes like authentication, rate-limiting and logging. 
    - Configure Routes: Define routes that match URLs and forward requests to downstream services. 
    - Filters: Use filters for custom logic, like authentication or request modification.
  
  ```java
    @Bean
    public RouteLocator customRouteLocator(RouteLocatorBuilder builder) {
        return builder.routes()
                .route(r -> r.path("/myService/**")
                .uri("lb://MY-SERVICE")
                .id("myServiceRoute"))
            .build();
    }
  ```

- **What is IOC? How many types of IOC?**
  There are two types of IOC like below - 
  - Bean Factory
  - ApplicationContext

- **What is Bean? How many ways we can create bean?**

- **Please explain bean lifecycle?**

- **What is Spring metadata? How many types of metadata are available?**

- **What is bean scope? How many scopes are there?**

- **Filter vs Interceptor? When we use what?**

- **@Component Vs @Bean?**

- **How to exclude any bean from auto-configuration?**

- **What is @RestController?**

- **Controller vs RestController?**

- **What is @SpringBootApplication annotation contains?**

- **Difference between war and tomcat server?**

- **How to get all beans of an application programmatically?**

- **Why we use @Profile?**

- **Why we use @Qualifier? Why it is different from @Primary?**