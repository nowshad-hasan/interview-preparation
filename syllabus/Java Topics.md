### Basics

- Overloading Vs Overriding
- 4 concepts of OOP (PIE) - Polymorphism, Inheritance, Encapsulation, Abstraction
- Abstract class vs interface
- Autoboxing Vs Unboxing
- Typecasting in Java, Upcasting, Downcasting
- Is Java Pass By reference or Pass by value
- Difference between local, instance and class variables
- 8 primitive types, their default value and memory allocation
- String pool, string.intern()
- StringBuffer Vs StringBuilder. StringJoiner
- Constructor Vs methods
- Why composition over inheritance (Has A vs Is A)
- Static method, static class, inner class
- Why main method static in java
- Why constructors can not be final and can not return values?
- Default, static method in interface.
- Why multiple inheritance not possible in java? What is diamond problem?
- Type of Interface variable
- Rules of method overloading. What's gonna happen when inheritance is applied to a method?
- When auto-constructor added and when not
- Use of `super`
- Power of `enum`
- Static variable, constant and method
- Access modifiers
- Constructor chaining
- Final class and final method - usage
- Abstract class and its usage, rules
- @override annotation
- Interface method rules
- try-catch
- try with resources
- finally block
- Exception vs error
- checked vs unchecked exception
- throw vs throws
- Best practice to write try-catch
- String concatenation best practices and why
- Command line arguments - args pass
- Object class
- String formatting
- Java reflection API
- Method Handles
- Java 17 features
- How object reference changed
- Interface's default methods, static method, private methods
- Deep cloning vs Shallow cloning . Understand with example.
- Copy constructor. How it is used in cloning?
- Can we pollute final methods or variables using Java Reflection API? 
- Upcasting and downcasting. (upcasting is natural, downcast is explicit and used with instanceof)
- What are limitation of abstract class? like - how method should be used? if final is possible in method name?
- What is JIT compiler? 
- What is AOT compiler?

### Java 8 special

- Anonymous inner class and lambda expression. Difference between these two.
- Different kinds of Programming Paradigm - Imperative, Declarative, Structured, Procedural, Functional, Object Oriented
- Method vs Function. Side Effect
- Imperative vs Declarative programming language
- Functional Interface
- Scope of lambda Expression
- Static method reference, Instance method reference, Constructor reference
- Default method and the solutions of multiple inheritance for interfaces
- Stream
- Collectors, Summarizing, String Joining, Grouping, Sub-grouping
- Exception handling for lambda expression
- Local type interference

### Generics

- subtyping
- bounded type
- wildcard argument
- generic method
- type erasure
- Math API
- Random number
- BigInteger, BigDecimal
- Unbounded type
- Upper bounded wildcard
- Lower bounded wildcard

### Java I/O and NIO

### Collection Framework

- Collection interface
- Array vs ArrayList
- Iterator vs enumeration
- Vector vs ArrayList
- HashMap Vs HashSet
- HashSet vs TreeSet vs LinkedHashSet
- HashMap vs TreeMap vs LinkedHashMap
- Stack vs Queue
- PriorityQueue
- Deque
- list -> set, set -> list
- the full diagram of collection framework
- HashMap vs HashTable
- Comparable interface and sorting in java
- searching
- Collection factory methods

### DateTime API

- LocalTime, LocalDate, LocalDateTime
- TimeZone, ZoneId, ZonedDateTime
- Formating, parsing

### JVM and GC

- What is GC? How does it work? Steps of GC.
- What is Java Memory Model? How are its' Heap and Stack organized?
- Explain Heap and Stack memory
- Minor GC, Major GC and Full GC
- What is memory leak? How does it happen? What is its solution?
- Class loading, class object
- Bytecode, bytecode instruction
- What is JIT compiler? How does it work better in JVM?
- What is the purpose of the finalize() method? Why it is deprecated?
- What is the Java Memory Model?
- Describe the different parts of the Java heap memory.
- What is garbage collection in Java?
- How does the garbage collector know which objects to collect?
- Explain the concept of “Stop-the-world” in Java garbage collection.
- What are the different types of references in Java?
- How does the JVM manage memory in terms of stack and heap?
- What is a memory leak in Java, and how can it be prevented?
- Explain the concept of the OutOfMemoryError in Java.
- Are There Any Disadvantages of Garbage Collection?
- When Does an Object Become Eligible for Garbage Collection? Describe How the Gc Collects an Eligible Object?
- How Do You Trigger Garbage Collection from Java Code?
- Describe Strong, Weak, Soft and Phantom References and Their Role in Garbage Collection.
- Suppose We Have a Circular Reference (Two Objects That Reference Each Other). Could Such Pair of Objects Become Eligible for Garbage Collection and Why?
- What JVM Parameters Are Commonly Used for Memory Management?
- What Are Memory Profiling Tools in Java? - VisualVM, Eclipse Memory Analyzer, JProfiler


### Threading

- What is threading
- What are the benefits of using Multithreading?
- Process vs Thread
- JStack, JConsole
- Lifecycle of a thread
- Thread creating, starting, pausing and terminating
- volaile keyword and in which cases it can be used?
- Thread sleeping, resuming
- How do you stop a thread in Java?
- Exception handling from thread
- ThreadLocal
- Memory share across multiple threads
- Immutable class
- Deadlock vs Livelock vs Starvation
- The Dining Philosophers Problem
- Wait(), notify() and notifyAll()
- Synchronized and concurrent collection
- BlockingQueue
- Executor framework
- Thread Pool and how to use it?
- Callable, Future
- Locks, latches
- Concurrency vs Parallelism
- Atomic variable
- Daemon Thread
- Data race (data issue -> use volatile and immutable object) vs race condition (like money deposit, withdraw condition -> use synchronised as volatile will not work here)
- What is the effect of ImmutableObject in thread safety?
- Is any other thread is gonna be ended when main thread is finished?
- What does `join()` method do?
- How to handle checked and unchecked exception while creating new thread?
- When use `synchronised`,  `synchronised(this)` and `synchronised(lock)`(Object lock = new Object())?
- How to use lock in static method?
- What is intrinsic and explicit lock?
- User thread vs daemon thread
- Runnable vs Callable
- How do threads communicate with each other? --- Using wait(), notify(), notifyAll()
- What is ConcurrentHashMap and Hashtable? In java, why is ConcurrentHashMap considered faster than Hashtable?
- Can you start a thread twice?
- Explain context switching.
- Explain CyclicBarrier, CountDownLatch, Semaphore
- What is a shutdown hook?
- Explain thread priority.
- Is it possible that each thread can have its stack in multithreaded programming?
- What is the lock interface? Why is it better to use a lock interface rather than a synchronized block?
- What is Thread Scheduler and Time Slicing?
- How can we make sure main() is the last thread to finish in Java Program?
- Why thread communication methods wait(), notify() and notifyAll() are in Object class?
- Why wait(), notify() and notifyAll() methods have to be called from synchronized method or block?
- Why Thread sleep() and yield() methods are static?
- What is Thread Group? Why it’s advised not to use it?
- What is atomic operation? What are atomic classes in Java Concurrency API?
- What Are Executor and Executorservice? What Are the Differences Between These Interfaces?
- Describe the Purpose and Use-Cases of the Fork/Join Framework.
- If Two Threads Call a Synchronized Method on Different Object Instances Simultaneously, Could One of These Threads Block? What If the Method Is Static?
- What are the ways to achieve thread safety in Java?
- Difference between execute() and submit() methods in ExecutorService.
- Difference between a fixed thread pool and a cached thread pool?
- How does ThreadPoolExecutor work internally?
- What are the core and maximum pool sizes in ThreadPoolExecutor?
- How would you handle a scenario where you need to perform multiple tasks in parallel? - using thread pool
- What is the keep-alive time in ThreadPoolExecutor and how does it affect thread pool behavior?
- What's the difference between synchronous and asynchronous programming?
- What's time slicing?
