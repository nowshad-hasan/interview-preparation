# Common questions
- **What is microservice architecture?**
  - multiple process deployment for separate business concern. It is not about single codebase or multiple codebase. Main part is there will be specific contract for each microservice. So, if anything changes inside a service, it does not matter until the contract is broken. Overall, it is loosely coupled.
  
- **What is monolithic architecture?**
  - Just opposite of microservice. There will be one single mammoth deployment with all the business logic. So, if I need to stop one thing, I need to stop the whole process and restart it.

- **What are the advantages of microservice?**
  - Each service can be deployed, maintained and tested individually. Yes, deployment time for individual service is faster (For the first time when 10 different microservices need to be started, then it is slower). And a small team can take care of a single service. And we can build each microservice with different languages. Yes, there may be some limitations but it is possible in this architecture.

- **What is Spring Cloud?**
  - Spring Cloud is an umbrella where all the tools needed for microservice implementation with spring boot are situated. The tools are like - service discovery, fault tolerance, circuit breaker etc.

- **What are the tools used in Spring Boot microservice ecosystem?**
  - Service discovery with *Eureka*
  - Fault tolerance 
  - Circuit breaker with *Hystrix* 

- **What are the challenges using microservice?**
  - Complex monitoring, deployment. Even if any service has dependency with some other services, then these teams need to co-ordinate in them for release their features. And more operations needed to operate a microservice.

- **In which cases microservice architecture best suited?**
  - Very complex project where multiple teams are working on separate features. So, it is easy to write code, test and deploy without managing the full project in monolith. Another use case is - scaling. If any very specific service needs to scale up and scale down very frequently, then we can just do this without scaling the full application.
- **What are the test types in microservice?**
  - Unit test, Integration test, acceptance test (UAT, alpha testing, beta testing). And a little bit contract testing which ensures that a service's contract is not broken to other services.

- **Explain the use of PACT in Microservices architecture?**
  - It is a tool which used in contract testing in microservice. Let's say a service has a contract. So if that is provided in the PACT, then it ensures that this 'pact' is not broken to other services.

- **Why are container used in Microservices?**
  - Maybe a microservice needs specific environment. So, it is easy to deploy a docker-image in EC2 with all the requirements for the microservice. Or let's say we want to scale that microservice, deploy same instance into 10 different machines. So it is also easier with container deployment.

- **What is the meaning of semantic monitoring in Microservices architecture?**
  - *Semantic* means *meaning*. It means that we take a specific business flow, like - Checkout flow in an e-commerce application, and test or monitor the full flow. It may contain multiple services to test.

- **What is CDC pattern in microservice?**
  - CDC stands for Consumer-Driven-Contract. It defines that consumer will make the requirements clear with a contract and the service has to implement the contract accordingly. There are three concepts here, consumer, provider and contract. Consumer defines the contract, provider will give the contract and contract is the requirement like - api-endpoint, data-format etc.

- **What is Continuous Monitoring?**
  - It is like CI/CD. In microservice, we always need to monitor and check our services whether anything is broken.

- **What is API Gateway?**
  - In a large scale microservice application, it is the first entrypoint where all the client applications hit. A single entrypoint for all the microservices. So, it is a major part here. It does several works here. An example is Zuul by Netflix.
    - Authentication using any identity provider
    - Error handling 
    - Parameter validation 
    - Rate limiting
    - Load balancing and circuit breaking
    - Protocol translation and service discovery
    - Monitoring, logging, analytics 
    - Caching
    - Dynamic routing to specific service with service discovery
    - Protocol translation like gRPC
  - The disadvantages are - 
    - the full lifecycle is slow as every request go through this
    - we need to deploy multiple api-gateway so that no single-point-of-failure is happening
    - Maybe we also need to use load-balancer for api-gateway so that it does not burn out 
    - maybe it will be complicated configuration. Like - android, ios, web needs different type of api. Then we need to use separate api-gateway for different clients

- **What is service discovery?**

- **What is Service Mesh?**
  - Istio is a open source service mesh tool. If there are few services, then service-mesh is a overkill. It is helpful for hundreds of services like Netflix. There are few key concepts for this pattern -
    - Secured communication between service with mutual TLS (mTLS).
    - Traffic management like load balancing or canary deployment
    - Retry mechanism and fallbacks
    - Observability like distributed tracing
    - Also used for service-discovery

- **What is bulkhead pattern?**
  - The name comes from ship's architecture for fault tolerance. Like - if water enters into one bottom compartment, does it sink the whole ship? No, it should not. Every bottom compartment should be isolated so that affected part does not do any harm to other compartments. But how this relates to microservice? Maybe service A is slow or down. But service B should not be down, it should be running up and ok. This is tbe main concept. But how to implement this? We can assign separate thread-pool with hystrix for each service, so that one service's heavy load does not effect to other service.

- **What is circuit breaker pattern?**
  - Resilience4J, Hystrix, Sentinel tool is used in spring boot. In this pattern we need to save the full system being burned down for a simple burnout service. And in electrical concept, circuit breaker is different from fuse. Fuse is totally burnt and need to be replaced where circuit breaker is just down automatically and then either manual or automatic intervention, that part need to be resumed again. There are 3 steps here -
    - Open - 
    - Half-open - 
    - Closed -  
 - In microservice for this pattern - 
    - Detect something wrong
    - Take temporary steps to avoid the situations getting worse
    - Deactivate the 'problem' component so that it does not affect downstream components and down the full system

- **What are the fault tolerance pattern in microservice?**
  - Circuit breaker pattern - Preventing Repeated Failures
  - Retry pattern - Handling Temporary Failures with Exponential Backoff
  - Fallback pattern - Providing Alternative Responses
  - Bulkhead pattern - Isolating Failures to Protect Critical Services
  - TImeout pattern - Ensuring Your System Remains Responsive

- **What is Event Driven Architecture pattern?**
  - It is a pattern where services communicate via a message broker. Here publisher publishes a task in the message queue and the responsible service (consumer) gets the task and perform that. So, there is no one-to-one communication between services. It is helpful for email sending, or auditing or any background job. There are few advantages - 
    - It decouples the component, as two services does not bother about their task --all they need to publish and consume. And if any new service comes up, it will just subscribe to the message broker. And that's it. Nothing to work with any other service. And if any service goes down, it does not bother other services at all. 
    - It is dependency inversion. Producer service does not directly work with low-level services. Both services are dependent on the abstraction layer named - message broker.
    - It is scalable. We can add more subscribers for a single event without much more hustle.
  - There are disadvantages as well - 
    - When multiple services fired up for single event, then it is a challenge to make the data consistent across those services. We can make it `Eventual consitent`. But this can also some problems like - for an e-commerce application, two users may order same last item as both are seeing data from different services. 
    - Duplicate message - Actually message broker keeps tract of the message being kept up any service. But if the service goes down with some ahead 2 message, but the tracker is behind 2 message, then the service after going live, will start from tracker's message which is 2 message behind. To reduce this problem, we need to make each subscriber is `idempotent`. And each message should contain unique-id so that any message should not be processed twice. 
    - More and more complex. So, harder to debug.
  
- **Is there any other way on how can services communicate without rest api?**
  - Yes, they can communicate via message broker, like - rabbitMQ, Kafka. It is called event-driven architecture where all services will be subscribed to a message broker. So, any new event published by and service, then that particular service will be notified and get the task done.

- **What is Sidecar pattern?**
  - The name comes from a sidecar attached to a motorcycle. The motorcycle does the main job taking the rider. But the attached sidecar is doing something else which is very important but not connected to the main business. Same thing happens for sidecar pattern as well. The sidecar service runs alongside the main application handles different things like - logging, monitoring, proxying, security, traffic routing, service discovery, configuration management etc. It does not touch the core business logic. But yes, it takes the resource from the same machine and disk the main application runs on. Some advantages are - 
    - Decoupling from main application
    - This sidecar can evolve independently
    - Polyglot - each sidecar service can be written in separate language and framework
    - simplified maintenance
    - Improved observability
  - Some disadvantages are - 
    - Latency - it slows down a little bit as now it is a separate service
    - Complexity - it is now more and more complex setup

- **What is Strangler pattern?**
  - This pattern is used when a large scale monolith application is trying to convert to a microservice application. But how to do this migration? At first we need to identify the most valuable part of that application and make that a separate service. Then we can apply a `facade pattern` (basically a proxy) above the main application and the new service. It will decide which one to call for which url. So, in that time both microservice and monolith application exists. Gradually the monolith application will be replaced by the microservice application.

- **What is Saga pattern?**-
  - This pattern ensures *transaction* between multiple services. If it is a monolith application with single central database, we will have nothing to do. Our database and application will support the ACID property automatically. But in microservice world, there are separate database for separate service. So, how can we ensure that if anything goes wrong in the process flow, every previously taken steps must be rolled back as their old state? In that case Saga Pattern comes into play. There are two ways to implement this. Let's say we have an e-commerce application where there is a flow, order - payment.
    - Orchestration - It is a separate service where it tracks down every steps of the flow. If anything goes wrong, this service will roll back everything manually. Like - let's say order is done, so this service will note that down, then payment is initiated, again, it will be noted - now if payment is failed, then that will also be noted to Orchestra and it will release the product to the inventory. But if payment is success, Orchestra will be notified also and send command to notification service to sending main, sms and push. So, here a single orchestra is managing the full transaction flow. Some advantages are - Clear control flow, Easy to debugging. And disadvantages are - single point of failure, tightly coupled.
    - Choreography - It is based on event-driven architecture. Here a message broker (like - Kafka) will take care the transaction. Let's say order is done, then it will be notified to the broker and then broker will notify the payment service to initiate a process. If transaction is success, then broker will be notified again, and start another service action. But if the payment is failed, then it will trigger another event in order service to release the product in inventory. Advantages are - loosely coupled, better scalability. Disadvantages are - complex implementation and very hard to debug.

- **What is CQRS pattern?**
  - CQRS stands for Command Query Responsibility Segregation. The definition is - Command is like - Create, update and delete resources -- all the post methods, where Query - get the resources - the get method. Sometimes doing all the CRUD operations in the same service and in the same database overloads. Then this pattern comes into play. Here, we can break the single service into two components where one component will handle the Command and other will handle the Query. We may also separate the database for- the two services as well. The advantage is - it splits read and write into two different systems. Like - SQL for write, NoSQL for read. So, it scales very well if needed. It goes very well in event-driven architecture. The main disadvantage is - it is very complex. If we can do our task with simple CRUD operations, we should never implement this. CQRS should be the last resort for use. Another disadvantage is - data consistency. When we are maintaining two database for the same data, we must update read-database when there is a change in write-database. It can be done with event-driven pattern. Event Bus is a great tool for this. We can call this system `Eventual Consistent`.