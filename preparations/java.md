## Contents

 - [Basic](#basic)
 - [JVM](#jvm)
 - [OOP](#oop)
 - [Collections and Generics](#collections-and-generics)
 - [Objects and Primitives](#objects-and-primitives)
 - [Java Memory Model and Garbage Collector](#java-memory-model-and-garbage-collector)
 - [Others](#others)
 - [Collection](#collection)
 - [Read more](#read-more)

### Basic

 * <b>Why is Java said to be platform independent?</b></br>
    - The execution of the code does not depend upon the OS.</br>

* <b>Why is the main method static in java?</b></br>

    * The method is static because otherwise there would be ambiguity on which method to be called. If static is removed from the main method, Program compiles successfully . But at runtime throws an error “NoSuchMethodError”.
    * We can overload the main method in Java. But the program doesn’t execute the overloaded main method when we run your program, we need to call the overloaded main method from the actual main method only. To run a method without calling this main method, we would need to execute a static block.
    * In order to avoid NoSuchMethodError, we can call System.exit(0) after the static method.
    * Note: Any method declared static will be executed even before the main class is executed.
    * Example:
       ``` java
       public class Hello {
           static {
            System.out.println("Hello, World!");
           }
         }
         ```
       </br>

  Read more: [Stackoverflow](https://stackoverflow.com/questions/146576/why-is-the-java-main-method-static), [GeeksforGeeks](https://www.geeksforgeeks.org/understanding-static-in-public-static-void-main-in-java/)


* **Java Platforms**

  There are four platforms of the Java programming language:

  * Java Platform, Standard Edition (Java SE)

  * Java Platform, Enterprise Edition (Java EE)

  * Java Platform, Micro Edition (Java ME)

  * JavaFX </br>

  Read more: [Oracle](https://docs.oracle.com/javaee/6/firstcup/doc/gkhoy.html), [Stackoverflow](https://stackoverflow.com/questions/2857376/difference-between-java-se-ee-me), [Packtpub](https://subscription.packtpub.com/book/application_development/9781787127944/1/ch01lvl1sec12/java-editions)

### JVM

* **Some nice blogs for understanding JVM architecture.**
  - [JVM Blog](http://www.artima.com/insidejvm/ed2/jvm.html)
  - [Roseindia](http://www.roseindia.net/java/java-virtual-machine.shtml)
  - [interviewjava](http://www.interviewjava.com/2007/04/inside-java-virtual-machine.html)
  - [Javabeat](http://www.javabeat.net/2010/08/jvmjrejava-compiler-interview-questions/2/)
  - [JVM at Google](https://www.youtube.com/watch?v=DjOcfkhTZkM&t)


* **What is Java Virtual Machine?** [Guru99](https://www.guru99.com/java-virtual-machine-jvm.html), [GeeksforGeeks](https://www.geeksforgeeks.org/jvm-works-jvm-architecture/), [Javatpoint](https://www.javatpoint.com/internal-details-of-jvm), [Javaworld](https://www.javaworld.com/article/3272244/what-is-the-jvm-introducing-the-java-virtual-machine.html)

* **Explain the Difference amongst JVM Specification, JVM Implementation, JVM Runtime.** [GeeksforGeeks](https://www.geeksforgeeks.org/differences-jdk-jre-jvm/), [Stackoverflow](https://stackoverflow.com/questions/2097189/what-is-the-difference-amongst-jvm-spec-jvm-implementation-jvm-runtime)

* **Why is the source file named after the class?** [GeeksforGeeks](https://www.geeksforgeeks.org/myth-file-name-class-name-java/), [Blog](https://netjs.blogspot.com/2015/04/why-file-name-and-class-name-same-in-java.html), [Quora](https://www.quora.com/Why-does-java-file-name-must-be-same-as-public-class-name)

* **Where is my compiled class file?** [GeeksforGeeks 1](https://www.geeksforgeeks.org/java-class-file/), [GeeksforGeeks 2](https://www.geeksforgeeks.org/run-java-class-file-different-directory/)


 ### OOP

 * **Explain OOP Concepts.**

   > Object-Oriented Programming is a methodology of designing a program using classes, objects, inheritance, polymorphism,  abstraction, and encapsulation.

   - Inheritance [GeeksforGeeks](https://www.geeksforgeeks.org/inheritance-in-java/)
   - Polymorphism [GeeksforGeeks](https://www.geeksforgeeks.org/polymorphism-in-java/)
   - Encapsulation [GeeksforGeeks](https://www.geeksforgeeks.org/encapsulation-in-java/)
   - Abstraction [GeeksforGeeks](https://www.geeksforgeeks.org/abstraction-in-java-2/)<br/>
    <br/>
 * **Differences between abstract classes and interfaces?** [GeeksforGeeks](https://www.geeksforgeeks.org/difference-between-abstract-class-and-interface-in-java/)

   - An abstract class, is a class that contains both concrete and abstract methods
   (methods without implementations). An abstract method must be implemented by the abstract class
    sub-classes. Abstract classes cannot be instantiated and need to be extended to be used.
   - Abstract class can have final, non-final, static and non-static variables. Interface has only static and final variables.<br/>
<br/>

 * <b>What is Abstract class?</b></br>
   * Abstract classes are classes that contain one or more abstract methods. An abstract method is a method that is declared, but contains no implementation.
   * If even a single method is abstract, the whole class must be declared abstract.
   * Abstract classes may not be instantiated, and require subclasses to provide implementations for the abstract methods.
   * You can’t mark a class as both abstract and final.
   * Non-abstract methods can access a method that you declare as abstract.</br>

   Read more: [GeeksforGeeks](https://www.geeksforgeeks.org/abstract-classes-in-java/), [JavatPoint](https://www.javatpoint.com/abstract-class-in-java), [Oracle](https://docs.oracle.com/javase/tutorial/java/IandI/abstract.html)

* <b>What are Interfaces?</b></br>
  * Interfaces are only declared methods that an implementing class would need.
  * Interfaces cannot be marked as final. Interface variables must be static or final.
  * Interfaces cannot be instantiated directly.
  * <b>Marker Interfaces</b>: Marker interfaces are those which do not declare any required Methods. The java.io.Serializable interface is a typical marker interfaces. These do not contain any methods, but classes must implement this interface in order to be serialized and de-serialized.</br></br>

  Read more: [JavatPoint](https://www.javatpoint.com/interface-in-java), [GeeksforGeeks](https://www.geeksforgeeks.org/interfaces-in-java/), [Guru99](https://www.guru99.com/java-interface.html), [Beginnersbook](https://beginnersbook.com/2013/05/java-interface/)

* **What is the difference between iterator and enumeration in java?** [Javaconceptoftheday](https://javaconceptoftheday.com/differences-between-enumeration-vs-iterator-in-java/), [Stackoverflow](https://stackoverflow.com/questions/948194/difference-between-java-enumeration-and-iterator)
    - **Fail-Fast Vs Fail-Safe** - Iterator is a fail-fast in nature. i.e it throws ConcurrentModificationException if a collection is modified while iterating other than it’s own remove() method. Where as Enumeration is fail-safe in nature. It doesn’t throw any exceptions if a collection is modified while iterating. [See more](https://javaconceptoftheday.com/fail-fast-and-fail-safe-iterators-in-java-with-examples/)

    - **Safe And Secure** - As Iterator is fail-fast in nature and doesn’t allow modification of a collection by other threads while iterating, it is considered as safe and secure than Enumeration.

    - **Which One To Use** - According to Java API Docs, Iterator is always preferred over the Enumeration. Here is the note from the Enumeration Docs.

      NOTE: *The functionality of this interface is duplicated by the Iterator interface. In addition, Iterator adds an optional remove operation, and has shorter method names. New implementations should consider using Iterator in preference to Enumeration.*

* **Do you agree we use composition over inheritance?**  

    The `java.util.Properties` class is a good example of a bad use of inheritance. Rather than using a Hashtable to store its properties, it extends Hashtable, in order to reuse its methods and to avoid reimplementing some of them using delegation. </br>
    Read more - [Journaldev](https://www.journaldev.com/12086/composition-vs-inheritance), [Baeldung](https://www.baeldung.com/java-inheritance-composition), [Stackoverflow](https://stackoverflow.com/questions/11343840/favor-composition-over-inheritance), [Dzone](https://dzone.com/articles/how-to-customize-serialization-in-java-using-the-e)</br>
    Video - [Fun Fun Function](https://www.youtube.com/watch?v=wfMtDGfHWpA)

* <b>What is Method overloading?</b></br>
     * Method Overloading means to have two or more methods with same name in the same class with different arguments.
     * Note:
       * Overloaded methods MUST change the argument list
       * Overloaded methods CAN change the return type
       * Overloaded methods CAN change the access modifier
       * Overloaded methods CAN declare new or broader checked exceptions
       * A method can be overloaded in the same class or in a subclass </br>

    Read more: [Beginnersbook](https://beginnersbook.com/2013/05/method-overloading/), [JavatPoint](https://www.javatpoint.com/method-overloading-in-java), [GeeksforGeeks](https://www.geeksforgeeks.org/overloading-in-java/)

* <b>What is Method overriding?</b></br>
     * Method overriding occurs when sub class declares a method that has the same type arguments as a method declared by one of its superclass
     * You can’t override a method marked public and make it protected
     * You cannot override a method marked final
     * You cannot override a method marked static
     * Note: Static methods cannot be overridden. Overloaded methods can still be overridden. </br>

   Read more: [GeeksforGeeks](https://www.geeksforgeeks.org/overriding-in-java/), [JavatPoint](https://www.javatpoint.com/method-overriding-in-java), [Beginnersbook](https://beginnersbook.com/2014/01/method-overriding-in-java-with-example/)</br></br>

* <b>Why would you not call abstract method in constructor?</b></br>
     The problem is that the class is not yet fully initialized, and when the method is called in a subclass, it may cause trouble.</br>

* <b>Constructors vs Methods? [GeeksforGeeks](https://www.geeksforgeeks.org/difference-between-the-constructors-and-methods/) </b></br>
   <b>Constructors:</b> Constructors must have the name as the class name and does not have a return type. It can be used to instantiate any objects in the class whereas methods have no such rule and is another member of the class. Constructors cannot be inherited but a derived class can call the super constructor of parent class.
     * ```this()```: Constructors use this to refer to another constructor in the same class with a different parameter list.
     * ```super()```: Constructors use super to invoke the superclass's constructor.

   <b>Methods:</b> Instance methods on the other hand require an instance of the class to exist before they can be called, so an instance of a class needs to be created by using the new keyword. Class methods are methods which are declared as static. The method can be called without creating an instance of the class</br>

* <b>Difference between Encapsulation & Abstraction?</b> [Guru99](https://www.guru99.com/difference-between-abstraction-and-encapsulation.html), [Javarevisited](https://javarevisited.blogspot.com/2017/04/difference-between-abstraction-and-encapsulation-in-java-oop.html)</br>
     * <b>Abstraction</b> focuses on the outside view of an object (i.e. the interface)
     * <b>Encapsulation</b> (information hiding) prevents clients from seeing it’s inside view.
     * Abstraction solves the problem in the design side while Encapsulation is the Implementation.</br>  
* **Difference between method overloading and overriding.**
          <p align="center">
          <img alt="Overloading and Overriding" src="https://github.com/codeshef/android-interview-questions/blob/master/assets/overloading-vs-overriding.png">
          </p>
    - Overloading happens at compile-time while Overriding happens at runtime: The binding of overloaded method call to its definition happens at compile-time however binding of overridden method call to its definition happens at runtime.
      More info on static vs. dynamic binding: [StackOverflow](https://stackoverflow.com/questions/19017258/static-vs-dynamic-binding-in-java).
    - Static methods can be overloaded which means a class can have more than one static method of same name. Static methods cannot be overridden, even if you declare a same static method in child class it has nothing to do with the same method of parent class as overridden static methods are chosen by the reference class and not by the class of the object.

        So, for example:
        ```java
          public class Animal {
              public static void testClassMethod() {
                  System.out.println("The static method in Animal");
              }

              public void testInstanceMethod() {
                  System.out.println("The instance method in Animal");
              }
          }

          public class Cat extends Animal {
              public static void testClassMethod() {
                  System.out.println("The static method in Cat");
              }

              public void testInstanceMethod() {
                  System.out.println("The instance method in Cat");
              }

              public static void main(String[] args) {
                  Cat myCat = new Cat();
                  myCat.testClassMethod();
                  Animal myAnimal = myCat;
                  myAnimal.testClassMethod();
                  myAnimal.testInstanceMethod();
              }
          }
          ```
          Will output:
          ```java
          The static method in Cat    // testClassMethod() is called from "Cat" reference

          The static method in Animal // testClassMethod() is called from "Animal" reference,
                                      // ignoring actual object inside it (Cat)

          The instance method in Cat  // testInstanceMethod() is called from "Animal" reference,
                                      // but from "Cat" object underneath
        ```

        The most basic difference is that overloading is being done in the same class while for overriding base and child classes are required. Overriding is all about giving a specific implementation to the inherited method of parent class.

        Static binding is being used for overloaded methods and dynamic binding is being used for overridden/overriding methods.
        Performance: Overloading gives better performance compared to overriding. The reason is that the binding of overridden methods is being done at runtime.

        Private and final methods can be overloaded but they cannot be overridden. It means a class can have more than one private/final methods of same name but a child class cannot override the private/final methods of their base class.

        Return type of method does not matter in case of method overloading, it can be same or different. However in case of method overriding the overriding method can have more specific return type (meaning if, for example, base method returns an instance of Number class, all overriding methods can return any class that is extended from Number, but not a class that is higher in the hierarchy, like, for example, Object is in this particular case).

        Argument list should be different while doing method overloading. Argument list should be same in method Overriding.

        It is also a good practice to annotate overridden methods with `@Override` to make the compiler be able to notify you if child is, indeed, overriding parent's class method during compile-time.

* <b>What is Encapsulation?</b></br>
    * Encapsulation involves binding code and data together as a single unit.
    * Encapsulation is a technique used for hiding the properties and behaviors of an object and allowing outside access only as appropriate. It prevents other objects from directly altering or accessing the properties or methods of the encapsulated object.
    * For instance, a class can be an encapsulated class if all the variables in it are defined as Private and by providing getter and setter methods.
  </br>


* **What is Polymorphism? What about Inheritance?**
  - Polymorphism in Java has two types: Compile time polymorphism (static binding) and Runtime polymorphism (dynamic binding). Method overloading is an example of static polymorphism, while method overriding is an example of dynamic polymorphism.

	 An important example of polymorphism is how a parent class refers to a child class object.  In fact, any object that satisfies more than one IS-A relationship is polymorphic in nature.

	 For instance, let’s consider a class `Animal` and let `Cat` be a subclass of `Animal`. So, any cat IS animal. Here, Cat satisfies the IS-A relationship for its own type as well as its super class Animal.

  - Inheritance is the process by which objects of one class acquire the properties & objects of another class. The two most common reasons to use inheritance are: a) To promote code reuse. b) To use polymorphism.

  - Inheritance can be defined as the process where one class acquires the properties (methods and fields) of another. With the use of inheritance the information is made manageable in a hierarchical order.

	 The class which inherits the properties of other is known as subclass (derived class, child class) and the class whose properties are inherited is known as superclass (base class, parent class).

	 Inheritance uses the keyword `extends` to inherit the properties of a class. Following is the syntax of extends keyword.
	 ```java
	 class Super {
	   .....
	   .....
  	}
	 class Sub extends Super {
	   .....
	   .....
	 }
	 ```

* **Multiple inheritance in Classes and Interfaces in java** [Blog](http://codeinventions.blogspot.in/2014/07/can-interface-extend-multiple.html), [GeeksforGeeks](https://www.geeksforgeeks.org/java-and-multiple-inheritance/)</br>

  Java supports multiple inheritance by interface only since it can implement multiple interfaces but can extend only one class.

  Language that supports multiple inheritance - [C++](https://www.geeksforgeeks.org/multiple-inheritance-in-c/), [Python](https://www.programiz.com/python-programming/multiple-inheritance)


### Collections and Generics

  - Arrays vs ArrayLists [GeeksforGeeks](https://www.geeksforgeeks.org/array-vs-arraylist-in-java/),
    [Quora](https://www.quora.com/What-is-the-difference-between-an-array-and-an-array-list),
    [Blog](https://javahungry.blogspot.com/2015/03/difference-between-array-and-arraylist-in-java-example.html)
  - HashSet vs TreeSet [Stackoverflow](https://stackoverflow.com/questions/25602382/java-hashset-vs-treeset-when-should-i-use-over-other/25602519), [GeeksforGeeks](https://www.geeksforgeeks.org/hashset-vs-treeset-in-java/),
     [Baeldung](https://www.baeldung.com/java-hashset-vs-treeset)
  - HashSet vs. TreeSet vs. LinkedHashSet [Blog 1](https://javarevisited.blogspot.com/2012/11/difference-between-treeset-hashset-vs-linkedhashset-java.html), [Blog 2](https://www.programcreek.com/2013/03/hashset-vs-treeset-vs-linkedhashset/), [Blog 3](https://javaconceptoftheday.com/hashset-vs-linkedhashset-vs-treeset-in-java/), [Stackoverflow](https://stackoverflow.com/questions/20116660/hashset-vs-treeset-vs-linkedhashset-on-basis-of-adding-duplicate-value), [GeeksforGeeks](https://www.geeksforgeeks.org/difference-and-similarities-between-hashset-linkedhashset-and-treeset-in-java/), [DZone](https://dzone.com/articles/hashset-vs-treeset-vs)
  - HashMap vs Set [Stackoverflow](https://stackoverflow.com/questions/2773824/difference-between-hashset-and-hashmap), [GeeksforGeeks](https://www.geeksforgeeks.org/difference-between-hashmap-and-hashset/)
  - HashMap and TreeMap [GeeksforGeeks](https://www.geeksforgeeks.org/hashmap-treemap-java/), [Baeldung](https://www.baeldung.com/java-treemap-vs-hashmap), [DZone](https://dzone.com/articles/hashmap-vs-treemap-vs)
  - ArrayList vs. HashMap [GeeksforGeeks](https://www.geeksforgeeks.org/arraylist-vs-hashmap-in-java/)
  - Stack vs Queue [GeeksforGeeks](https://www.geeksforgeeks.org/difference-between-stack-and-queue-data-structures/)

  * **Explain Generics in Java?**
      - Generics were included in Java language to provide stronger type checks, by allowing the programmer to define, which classes can be used with other classes
           > In a nutshell, generics enable types (classes and interfaces) to be parameters when defining classes, interfaces and methods. Much like the more familiar formal parameters used in method declarations, type parameters provide a way for you to re-use the same code with different inputs. The difference is that the inputs to formal parameters are values, while the inputs to type parameters are types. ([Official Java Documentation](https://docs.oracle.com/javase/tutorial/java/generics/why.html))

      - This means that, for example, you can define:
           ```java
           List<Integer> list = new ArrayList<>();
           ```
           And let the compiler take care of noticing, if you put some object, of type other than `Integer` into this list and warn you.
      - It should be noted that standard class hierarchy *does not* apply to generic types. It means that `Integer` in `List<Integer>` is not inherited from `<Number>` - it is actually inherited directly from `<Object>`. You can still put some constraints on what classes can be passed as a parameter into a generic by using [wildcards](https://docs.oracle.com/javase/tutorial/extra/generics/wildcards.html) like `<?>`, `<? extends MyCustomClass>` or `<? super Number>`.
      - While generics are very useful, late inclusion into Java language has put some restraints on their implementation - backward compatibility required them to remain just "syntactic sugar" - they are erased ([type erasure](https://docs.oracle.com/javase/tutorial/java/generics/erasure.html)) during compile-time and replaced with `object` class.

      * Before generics, we can store any type of objects in collection i.e. non-generic. Now generics, forces the java programmer to store specific type of objects.
      * Type-safety : We can hold only a single type of objects in generics. It doesn’t allow to store other objects.
      * Type casting is not required: There is no need to typecast the object.
      * Compile-Time Checking: It is checked at compile time so problem will not occur at runtime. The good programming strategy says it is far better to handle the problem at compile time than runtime.
      * Before Generics, we need to type cast.
      ```java
      List list = new ArrayList();  
      list.add("hello");  
      String s = (String) list.get(0); //typecasting  
      ```
      * After Generics, we don't need to typecast the object.
       ```java
       List<String> list = new ArrayList<String>();  
       list.add("hello");  
       String s = list.get(0);  
       ```
      * A class that can refer to any type is known as generic class. Here, we are using T type
   parameter to create the generic class of specific type. The T type indicates that it can refer to any type (like String, Integer, Employee etc.).The type you specify for the class, will be used to store and retrieve the data.
      * The ? (question mark) symbol represents wildcard element. It means any type. If we write <? extends Number>, it means any child class of Number e.g. Integer, Float, double etc

* **What is Java `PriorityQueue`?** [GeeksforGeeks](https://www.geeksforgeeks.org/priority-queue-class-in-java-2/), [Blog](https://www.callicoder.com/java-priority-queue/), [Javapoint](https://www.javatpoint.com/java-priorityqueue)

### Objects and Primitives

 * String vs StringBuffer vs StringBuilder - [GeeksforGeeks](https://www.geeksforgeeks.org/string-vs-stringbuilder-vs-stringbuffer-in-java/)
 * StringJoiner -  [GeeksforGeeks](https://www.geeksforgeeks.org/use-stringjoiner-stringbuilder/), [Baeldung](https://www.baeldung.com/java-string-joiner)
 * String concatenation techniques- [Baeldung](https://www.baeldung.com/java-strings-concatenation)
 * **How is `String` class implemented? Why was it made immutable?**

   There is no primitive variant of `String` class in Java language - all strings are just wrappers around underlying array of characters, which is declared `final`. This means that, once a `String` object is instantiated, it cannot be changed through normal tools of the language (Reflection still can mess things up horribly, because in Java no object is truly immutable). This is why `String` variables in classes are the first candidates to be used, when you want to override `hashCode()` and `equals()` of your class - you can be sure, that all their required contracts will be satisfied.
    > Note: The String class is immutable, so that once it is created a String object cannot be changed. The String class  has a number of methods, some of which will be discussed below, that appear to modify strings. Since strings are  immutable, what these methods really do is create and return a new string that contains the result of the operation. ([Official Java Documentation](https://docs.oracle.com/javase/tutorial/java/data/strings.html))

    This class is also unique in a sense, that, when you create an instance like this:
    ```java
    String helloWorld = "Hello, World!";
    ```
    `"Hello, World!"` is called a *literal* and compiler creates a `String` object with its' value. So
    ```java
    String capital = "Hello, World!".toUpperCase();
    ```
    is a valid statement, that, firstly, will create an object with literal value "Hello, World!" and then will create and return another object with value "HELLO, WORLD!"
  - `String` was made immutable to prevent malicious manipulation of data, when, for example, user login or other sensitive data is being send to a server.

* **What does it means to say that a `String` is immutable?**

    It means that once created, `String` object's `char[]` (its' containing value) is declared `final` and, therefore, it can not be changed during runtime.


* **What is `String.intern()`? When and why should it be used?** [Stackoverflow](https://stackoverflow.com/questions/10578984/what-is-java-string-interning), [GeeksforGeeks](https://www.geeksforgeeks.org/interning-of-string/)

* <b>String manipulation</b>
  [Baeldung](https://www.baeldung.com/java-string-interview-questions),
   [dev.to](https://dev.to/javinpaul/top-20-string-coding-problems-from-programming-job-interviews-493m),
   [Javatpoint](https://www.javatpoint.com/java-string-faqs),
   [Journaldev](https://www.journaldev.com/1321/java-string-interview-questions-and-answers)

* <b>String pool in Java:</b></br>
   * String Pool in java is a pool of Strings stored in Java Heap Memory.
   * When we use double quotes to create a String, it first looks for String with same value in the String pool, if found it just returns the reference else it creates a new String in the pool and then returns the reference.
   * However using new operator, we force String class to create a new String object in heap space. We can use intern() method to put it into the pool or refer to other String object from string pool having same value.
   * For example, how many strings are getting created in below statement;
  `String str = new String("Cat");`
   * In above statement, either 1 or 2 string will be created. If there is already a string literal “Cat” in the pool, then only one string “str” will be created in the pool. If there is no string literal “Cat” in the pool, then it will be first created in the pool and then in the heap space, so total 2 string objects will be created.</br>
   Read more: [Baeldung](https://www.baeldung.com/java-string-pool), [Journaldev](https://www.journaldev.com/797/what-is-java-string-pool), [Blog](https://study.com/academy/lesson/java-string-constant-pool-concept-mechanism.html)

* **Can you list 8 primitive types in java?** [GeeksforGeeks](https://www.geeksforgeeks.org/data-types-in-java/), [Baeldung](https://www.baeldung.com/java-primitives), [Oracle](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html)


* **What is the difference between an Integer and int?**

  `int` is a primitive data type (with `boolean`, `byte`, `char`, `short`, `long`, `float` and `double`), while `Integer` (with `Boolean`, `Byte`, `Character`, `Short`,`Long`, `Float` and `Double`) is a [wrapper](https://docs.oracle.com/javase/tutorial/java/data/numberclasses.html) class that encapsulates primitive data type, while providing useful methods to perform different tasks with it. Read more from [GeeksforGeeks](https://www.geeksforgeeks.org/difference-between-an-integer-and-int-in-java/). </br></br>

* **What is Autoboxing and Unboxing?**

  Autoboxing and Unboxing is the process of automatic wrapping (putting in a box) and unwrapping (getting the value out) of primitive data types, that have "wrapper" classes. So `int` and `Integer` can (almost always) be used interchangeably in Java language, meaning a method `void giveMeInt(int i) { ... }` can take `int` as well as `Integer` as a parameter. </br>

  Read more: [Oracle](https://docs.oracle.com/javase/tutorial/java/data/autoboxing.html), [GeeksforGeeks](https://www.geeksforgeeks.org/autoboxing-unboxing-java/)

* **Typecast in Java.**</br>
     In Java, you can use casts to polymorph one class into another, compatible one. For example:

     ```java
        long i = 10l;
        int j = (int) i;
        long k = j;
     ```
    Here we see, that, while narrowing (`long i` -> `int j`) requires an explicit cast to make sure the programmer realizes, that there may be some data or precision loss, widening (`int j` -> `long k`) does not require an explicit cast, because there can be no data loss (`long` can take larger numbers than `int` allows).


* **Do objects get passed by reference or value in Java? Elaborate on that.**

    In Java all primitives and objects are passed by value, meaning that their copy will be manipulated in the receiving method. But there is a caveat - when you pass an object reference into a method, a *copy of this reference* is made, so it still points to the same object. This means, that any changes that you make to the insides of this object are retained, when the method exits.
        ```java
        public class Pointer {

            int innerField;

            public Pointer(int a) {
                this.innerField = a;
            }
        }
        ```
        ```java
            public class ValueAndReference {

            public static void main(String[] args) {

                Pointer a = new Pointer(0);
                int b = 1;

                print("Before:");
                print("b = " + b);
                print("a.innerField = " + a.innerField);
                exampleMethod(a, b);
                print("After:");
                print("b = " + b);
                print("a.innerField = " + a.innerField);
            }

            static void exampleMethod(Pointer a, int b) {
                a.innerField = 2;
                b = 10;
            }

            static void print(String text) {
                System.out.println(text);
            }
        }
        ```
        Will output:
        ```java
            Before:

            b = 1

            a.innerField = 0

            After:

            b = 1        // a new local int variable was created and operated on, so "b" didn't change

            a.innerField = 2 // Pointer a got its' innerField variable changed
                             //  from 0 to 2, because method was operating on
                             //  the same reference to an instance
        ```

        Read more: [GeeksforGeeks](https://www.geeksforgeeks.org/g-fact-31-java-is-strictly-pass-by-value/), [Journaldev](https://www.journaldev.com/3884/java-is-pass-by-value-and-not-pass-by-reference),
         [Stackoverflow](https://stackoverflow.com/questions/40480/is-java-pass-by-reference-or-pass-by-value), [Mkyong](https://www.mkyong.com/java/is-java-pass-by-value-or-pass-by-reference/)
* **What is the difference between instantiation and initialization of an object?**
    - Initialization is the process of the memory allocation, when a new variable is created. Variables should be explicitly given a value, otherwise they may contain a random value that remained from the previous variable that was using the same memory space. To avoid this problem, Java language assigns default (right after initialization) values to some data types:
        * `boolean` defaults to `false`;
        * `byte` defaults to `0`;
        * `short` defaults to `0`;
        * `int` defaults to `0`;
        * `long` defaults to `0L`;
        * `char` defaults to `\u0000`;
        * `float` defaults to `0.0f`;
        * `double` defaults to `0.0d`;
        * `object` defaults to `null`.
    - Instantiation is the process of explicitly assigning definitive value to a declared variable:
        ```java
            int j;  // Initialized variable (int defaults to 0 right after)
            j = 10; // Instantiated variable
        ```

        Read more: [Oracle](https://docs.oracle.com/javase/tutorial/java/javaOO/objectcreation.html), [Stackoverflow](https://stackoverflow.com/questions/15074083/difference-between-initializing-a-class-and-instantiating-an-object), [Quora](https://www.quora.com/What-is-difference-between-Instantiate-and-Initialize-in-programming)

* **What the difference between local, instance and class variables?**
  - Local variables exist only in methods that created them, they are stored separately in their respected Thread Stack (for more information, see question about Java Memory Model) and cannot have their reference passed outside of the method scope. That also means that they cannot be assigned any access modifier or made `static` - because they only exist during enclosing method's execution and those modifiers just do not make sense, since no other outside method can get them anyway.
  - Instance variables are the ones, that are declared in classes and their value can be different from one instance of the class to another, but they always require that class' instance to exist.
  - Class variables are those, that are marked with `static` keyword in their class' body. They can only have one value across all instances of that class (changing it in one place will change it in their class and, therefore, in all instances) and can even be retrieved without that class' instance (if their access modifier allows it).</br>

  Read more: [Tutorialspoint](https://www.tutorialspoint.com/java/java_variable_types.htm), [GeeksforGeeks](https://www.geeksforgeeks.org/variables-in-java/), [Guru99](https://www.guru99.com/java-variables.html)

### Java Memory Model and Garbage Collector

* **What is garbage collector? How does it work?**</br>

   All objects are allocated on the heap area managed by the JVM.
  As long as an object is being referenced, the JVM considers it alive.
  Once an object is no longer referenced and therefore is not reachable by the application code,
  the garbage collector removes it and reclaims the unused memory. </br>
  Read more: [GeeksforGeeks](https://www.geeksforgeeks.org/garbage-collection-java/), [Oracle](https://www.oracle.com/webfolder/technetwork/tutorials/obe/java/gc01/index.html), [Baeldung](https://www.baeldung.com/jvm-garbage-collectors), [Journaldev](https://www.journaldev.com/16659/garbage-collection-in-java), [JavatPoint](https://www.javatpoint.com/Garbage-Collection), [Stackify](https://stackify.com/what-is-java-garbage-collection/)



* **What is Java Memory Model? What contracts does it guarantee? How are its' Heap and Stack organized?** [Jenkov](http://tutorials.jenkov.com/java-concurrency/java-memory-model.html), [Journaldev](https://www.journaldev.com/2856/java-jvm-memory-model-memory-management-in-java), [Medium](https://medium.com/platform-engineer/understanding-java-memory-model-1d0863f6d973), [Baeldung](https://www.baeldung.com/java-stack-heap), [Betsol](https://betsol.com/2017/06/java-memory-management-for-java-virtual-machine-jvm/), [GeeksforGeeks](https://www.geeksforgeeks.org/java-memory-management/)

  * Stack is used for static memory allocation and Heap for dynamic memory allocation, both stored in the computer's RAM .
  * Variables allocated on the stack are stored directly to the memory and access to this memory is very fast, and it's allocation is dealt with when the program is compiled. When a function or a method calls another function which in turns calls another function etc., the execution of all those functions remains suspended until the very last function returns its value. The stack is always reserved in a LIFO order, the most recently reserved block is always the next block to be freed. This makes it really simple to keep track of the stack, freeing a block from the stack is nothing more than adjusting one pointer.
  * Variables allocated on the heap have their memory allocated at run time and accessing this memory is a bit slower, but the heap size is only limited by the size of virtual memory . Element of the heap have no dependencies with each other and can always be accessed randomly at any time. You can allocate a block at any time and free it at any time. This makes it much more complex to keep track of which parts of the heap are allocated or free at any given time.
  * You can use the stack if you know exactly how much data you need to allocate before compile time and it is not too big. You can use heap if you don't know exactly how much data you will need at runtime or if you need to allocate a lot of data.
  * In a multi-threaded situation each thread will have its own completely independent stack but they will share the heap. Stack is thread specific and Heap is application specific. The stack is important to consider in exception handling and thread executions.
      * Heap memory is used by all the parts of the application whereas stack memory is used only by one thread of execution.
      * Whenever an object is created, it’s always stored in the Heap space and stack memory contains the reference to it. Stack memory only contains local primitive variables and reference variables to objects in heap space.
      * Objects stored in the heap are globally accessible whereas stack memory can’t be accessed by other threads.
      * Memory management in stack is done in LIFO manner whereas it’s more complex in Heap memory because it’s used globally. Heap memory is divided into Young-Generation, Old-Generation etc, more details at Java Garbage Collection.
      * Stack memory is short-lived whereas heap memory lives from the start till the end of application execution.
      * When stack memory is full, Java runtime throws java.lang.StackOverFlowError whereas if heap memory is full, it throws java.lang.OutOfMemoryError: Java Heap Space error.
      * Stack memory size is very less when compared to Heap memory. Because of simplicity in memory allocation (LIFO), stack memory is very fast when compared to heap memory.</br>   


* **Explain Java stack vs heap memory.** [Journaldev](https://www.journaldev.com/4098/java-heap-space-vs-stack-memory)

* **What is memory leak and how does Java handle it?**
[Baeldung](https://www.baeldung.com/java-memory-leaks), [Stackify](https://stackify.com/memory-leaks-java/), [DZOne](https://dzone.com/articles/what-memory-leak-java), [GeeksforGeeks](https://www.geeksforgeeks.org/memory-leaks-java/), [Plumbr](https://plumbr.io/blog/memory-leaks/what-is-a-memory-leak)
* **What are strong, soft, weak and phantom references in Java?** [DZone](https://dzone.com/articles/weak-soft-and-phantom-references-in-java-and-why-they-matter), [Stackoverflow](https://stackoverflow.com/questions/9809074/java-difference-between-strong-soft-weak-phantom-reference), [GeeksforGeeks](https://www.geeksforgeeks.org/types-references-java/), [Medium](https://medium.com/@ramtop/weak-soft-and-phantom-references-in-java-and-why-they-matter-c04bfc9dc792)

### Concurrency

* **What does the keyword `synchronized` mean?**
  * When you have two threads that are reading and writing to the same 'resource', say a variable named 'test', you need to ensure that these threads access the variable in an atomic way. Without the synchronized keyword, your thread 1 may not see the change thread 2 made to test.
  * <b>synchronized</b> blocks the next thread's call to method as long as the previous thread's execution is not finished. Threads can access this method one at a time.

  Read more: [Link](https://stackoverflow.com/a/1085745/2621950), [GeeksforGeeks](https://www.geeksforgeeks.org/synchronized-in-java/), [Baeldung](https://www.baeldung.com/java-synchronized), [JavaTPoint](https://www.javatpoint.com/synchronization-in-java)

* **What is AtomicBoolean in java?** [GeeksforGeeks](https://www.geeksforgeeks.org/atomicboolean-compareandset-method-in-java-with-examples/), [Jenkov](http://tutorials.jenkov.com/java-util-concurrent/atomicboolean.html)

* <b>What is ConcurrentLinkedQueue?</b> [GeeksforGeeks](https://www.geeksforgeeks.org/concurrentlinkedqueue-in-java-with-examples/), [Stackoverflow](https://stackoverflow.com/questions/616484/how-to-use-concurrentlinkedqueue), [Javatpoint](https://www.javatpoint.com/java-concurrentlinkedqueue)


* **What is a `ThreadPoolExecutor`?** [MindOrks](https://blog.mindorks.com/threadpoolexecutor-in-android-8e9d22330ee3), [Baeldung](https://www.baeldung.com/thread-pool-java-and-guava), [Journaldev](https://www.journaldev.com/1069/threadpoolexecutor-java-thread-pool-example-executorservice), [GeeksforGeeks](https://www.geeksforgeeks.org/thread-pools-java/)

* **What is `volatile` modifier?** [Jenkov](http://tutorials.jenkov.com/java-concurrency/volatile.html), [Stackoverflow](https://stackoverflow.com/questions/106591/what-is-the-volatile-keyword-useful-for), [GeeksforGeeks](https://www.geeksforgeeks.org/volatile-keyword-in-java/)

  * Suppose two threads are working on a method. If two threads run on different processors each thread may have its own local copy of variable. If one thread modifies its value the change might not reflect in the original one in the main memory instantly.
  * Now the other thread is not aware of the modified value which leads to data inconsistency.Essentially, volatile is used to indicate that a variable's value will be modified by different threads. “volatile” tells the compiler that the value of a variable must never be cached as its value may change outside of the scope of the program itself.
  * The value of this variable will never be cached thread-locally: all reads and writes will go straight to "main memory"
  * An access to a volatile variable never has the potential to block: we're only ever doing a simple read or write, so unlike a synchronized block we will never hold on to any lock.</br>


* <b>The clasess in the atomic package expose a common set of methods: `get`, `set,`, `lazyset`, `compareAndSet`, and `weakCompareAndSet`. Please describe them. </b>[Oracle](https://docs.oracle.com/javase/7/docs/api/java/util/concurrent/atomic/package-summary.html), [Baeldung](https://www.baeldung.com/java-atomic-variables)

### Exceptions

* **How does the `try{}  - catch{} - finally{}` works?** [Jenkov](http://tutorials.jenkov.com/java-exception-handling/basic-try-catch-finally.html), [GeeksforGeeks](https://www.geeksforgeeks.org/flow-control-in-try-catch-finally-in-java/)

* <b>Is there ever a scenario where we can skip the finally block in a try catch? [Stackoverflow](https://stackoverflow.com/questions/5579817/is-there-any-code-that-will-never-execute-finally-clause) </b></br>

     By Calling System.exit(0) in try or catch block, we can skip the finally block. System.exit(int) method can throw a SecurityException. If System.exit(0) exits the JVM without throwing that exception then finally block will not execute. But, if System.exit(0) does throw security exception then finally block will be executed.</br>


* **What is the difference between a `Checked Exception` and an `Un-Checked Exception`?** [GeeksforGeeks](https://www.geeksforgeeks.org/checked-vs-unchecked-exceptions-in-java/), [Stackoverflow](https://stackoverflow.com/questions/6115896/understanding-checked-vs-unchecked-exceptions-in-java), [Blog 1](https://howtodoinjava.com/java/exception-handling/checked-vs-unchecked-exceptions-in-java/), [Blog 2](https://crunchify.com/better-understanding-on-checked-vs-unchecked-exceptions-how-to-handle-exception-better-way-in-java/)

* <b>Difference between ‘throw’ and ‘throws’ in Java Exception Handling?</b></br>

    `throw` keyword is used to throw Exception from any method or static block whereas `throws` is used to indicate that which Exception can possibly be thrown by this method.</br>
   Read more: [Beginnersbook](https://beginnersbook.com/2013/04/difference-between-throw-and-throws-in-java/), [GeeksforGeeks 1](https://www.geeksforgeeks.org/throw-throws-java/), [GeeksforGeeks 2](https://www.geeksforgeeks.org/difference-between-throw-and-throws-in-java/)

### Others

* **What is serialization? How do you implement it?**
    - Serialization is the process of converting an object into a stream of bytes in order to store
    an object into memory, so that it can be recreated at a later time, while still keeping the
    object's original state and data. In Android you may use either the Serializable, Externalizable (implements Serializable) or Parcelable interfaces.
    - While Serializable is the easiest to implement, Externalizable may be used if you need to insert custom logic into the process of serialization (although it is almost never used nowadays as it is considered a relic from early versions of Java). But it is highly recommended to use Parcelable in Android instead, as Parcelable was created exclusively for Android and it performs about 10x faster than Serializable, because Serializable uses reflection, which is a slow process and tends to create a lot of temporary objects and it may cause garbage collection to occur more often.
    - To use Serializable all you have to do is implement the interface:

        ```java
        /**
        *  Implementing the Serializeable interface is all that is required
        */
        public class User implements Serializable {

            private String name;
            private String email;

                public User() {
                }

                public String getName() {
                    return name;
                }

                public void setName(final String name) {
                    this.name = name;
                }

                public String getEmail() {
                    return email;
                }

                public void setEmail(final String email) {
                    this.email = email;
                }
            }
        ```
</br>

   Read more: [GeeksforGeeks](https://www.geeksforgeeks.org/serialization-in-java/), [Baeldung](https://www.baeldung.com/java-serialization), [JavaTPoint](https://www.javatpoint.com/serialization-in-java), [DZone](https://dzone.com/articles/serialization-amp-de-serialization-in-java)

   * Parcelable requires a bit more work:

        ```java
            public class User implements Parcelable {

                private String name;
                private String email;

                /**
                 * Interface that must be implemented and provided as a public CREATOR field
                 * that generates instances of your Parcelable class from a Parcel.
                 */
                public static final Creator<User> CREATOR = new Creator<User>() {

                    /**
                     * Creates a new USer object from the Parcel. This is the reason why
                     * the constructor that takes a Parcel is needed.
                     */
                    @Override
                    public User createFromParcel(Parcel in) {
                        return new User(in);
                    }

                    /**
                     * Create a new array of the Parcelable class.
                     * @return an array of the Parcelable class,
                     * with every entry initialized to null.
                     */
                    @Override
                    public User[] newArray(int size) {
                        return new User[size];
                    }
                };

                public User() {
                }

                /**
                 * Parcel overloaded constructor required for
                 * Parcelable implementation used in the CREATOR
                 */
                private User(Parcel in) {
                    name = in.readString();
                    email = in.readString();
                }

                public String getName() {
                    return name;
                }

                public void setName(final String name) {
                    this.name = name;
                }

                public String getEmail() {
                    return email;
                }

                public void setEmail(final String email) {
                    this.email = email;
                }

                @Override
                public int describeContents() {
                    return 0;
                }

                /**
                 * This is where the parcel is performed.
                 */
                @Override
                public void writeToParcel(final Parcel parcel, final int i) {
                    parcel.writeString(name);
                    parcel.writeString(email);
                }
            }
        ```
        Note: For a full explanation of the <b>describeContents()</b> method see [StackOverflow](https://stackoverflow.com/questions/4076946/parcelable-where-when-is-describecontents-used/4914799#4914799).
        In Android Studio, you can have all of the parcelable code auto generated for you, but like with everything else, it is always a good thing to try and understand everything that is happening.
* **Parcelable vs Serializable** [Medium](https://android.jlelse.eu/parcelable-vs-serializable-6a2556d51538), [Stackoverflow](https://stackoverflow.com/questions/3323074/android-difference-between-parcelable-and-serializable)

* **What is `transient` modifier?** [JavaTPoint](https://www.javatpoint.com/transient-keyword), [GeeksforGeeks](https://www.geeksforgeeks.org/transient-keyword-java/), [Stackoverflow](https://stackoverflow.com/questions/910374/why-does-java-have-transient-fields), [Medium](https://medium.com/google-developer-experts/diving-deeper-into-the-java-transient-modifier-3b16eff68f42)

* **What are anonymous classes?** [OracleDoc](https://docs.oracle.com/javase/tutorial/java/javaOO/anonymousclasses.html), [Baeldung](https://www.baeldung.com/java-anonymous-classes), [GeeksforGeeks](https://www.geeksforgeeks.org/anonymous-inner-class-java/)

  * An anonymous class is just what its name implies -- it has no name. It combines the class declaration and the creation of an instance of the class in one step. Since anonymous classes have no name, objects can not be instantiated from outside the class in which the anonymous class is defined. In fact, an anonymous object can only be instantiated from within the same scope in which it is defined. </br>

  * Rules:
    * An anonymous class must always extend a super class or implement an interface but it cannot have an explicit extends or implements clause.
    * An anonymous class must implement all the abstract methods in the super class or the interface.
    * An anonymous class always uses the default constructor from the super class to create an instance.
    * Example:

    ```java
    MyButton.setOnClickListener(new Button.OnClickListener {
          @override
             public void onClick(View view){
                 //some code
             }
      });
    ```    
</br>

* **What is the difference between using `==` and `.equals` on an object?**  [GeeksForGeeks](http://www.geeksforgeeks.org/difference-equals-method-java/), [Stackoverflow](https://stackoverflow.com/questions/7520432/what-is-the-difference-between-and-equals-in-java)

   We can use == operators for reference comparison (address comparison) and .equals() method for content comparison. * In simple words, == checks if both objects point to the same memory location whereas .equals() evaluates to the comparison of values in the objects.


* **What is the `hashCode()` and `equals()` used for?** [Journaldev](https://www.journaldev.com/21095/java-equals-hashcode), [DZone](https://dzone.com/articles/working-with-hashcode-and-equals-in-java), [GeeksforGeeks](https://www.geeksforgeeks.org/equals-hashcode-methods-java/), [Baeldung](https://www.baeldung.com/java-equals-hashcode-contracts)

* **Why would you not call abstract method in constructor?** [Stackoverflow](https://stackoverflow.com/questions/15327417/is-it-ok-to-call-abstract-method-from-constructor-in-java)

* **When would you make an object value `final`?** [GeeksforGeeks 1](https://www.geeksforgeeks.org/final-vs-immutability-java/), [GeeksforGeeks 2](https://www.geeksforgeeks.org/final-keyword-java/)

* Final modifiers - once declared cannot be modified. A blank final variable in Java is a final variable that is not initialized during declaration.
   * final Classes- A final class cannot have subclasses.
   * final Variables- A final variable cannot be changed once it is initialized.
   * final Methods- A final method cannot be overridden by subclasses.</br>

   Read more: [JavatPoint](https://www.javatpoint.com/final-keyword)

* **What are these `final`, `finally` and `finalize` keywords?**
  - `final` is a keyword in the java language. It is used to apply restrictions on class, method and variable. Final class can't be inherited, final method can't be overridden and final variable value can't be changed.
	```java
	class FinalExample {
		public static void main(String[] args) {
			final int x=100;
			x=200;//Compile Time Error because x is final
		}
	}
	```
  - `finally` is a code block and is used to place important code, it will be executed whether exception is handled or not.
	```java
	class FinallyExample {
		public static void main(String[] args) {
			try {
				int x=300;
			}catch(Exception e) {
				System.out.println(e);
			}
			finally {
				System.out.println("finally block is executed");
			}
		}
	}
	```
  - `Finalize` is a method used to perform clean up processing just before object is garbage collected.
	```java
	class FinalizeExample {
		public void finalize() {
			System.out.println("finalize called");
		}

		public static void main(String[] args) {
			FinalizeExample f1=new FinalizeExample();
			FinalizeExample f2=new FinalizeExample();
			f1=null;
			f2=null;
			System.gc();
		}
	}
	```
Read more: [GeeksforGeeks](https://www.geeksforgeeks.org/g-fact-24-finalfinally-and-finalize-in-java/), [Baeldung](https://www.baeldung.com/java-final-finally-finalize)

* **What does the `static` word mean in Java?**</br>

     In case of `static` variable it means that this variable (its' value or the object it references) spans across all instances of enclosing class (changing it in one instance affects all others), while in case of `static` methods it means that these methods can be invoked without an instance of their enclosing class. It is useful, for example, when you create util classes that need not be instantiated every time you want to use them. </br>
Read more: [Baeldung](https://www.baeldung.com/java-static), [JavaTPoint](https://www.javatpoint.com/static-keyword-in-java), [GeeksforGeeks](https://www.geeksforgeeks.org/static-keyword-java/), [Final Static](https://www.geeksforgeeks.org/final-static-variable-java/), [Javarevisited](https://javarevisited.blogspot.com/2011/11/static-keyword-method-variable-java.html)


* **Can a `static` method be overridden in Java?** [GeeksforGeeks](https://www.geeksforgeeks.org/can-we-overload-or-override-static-methods-in-java/)</br>

   While child class can override a static method with another static method with the same signature (return type can be downcasted), it is not truly overridden - it becomes "hidden", but both methods can still be accessed under right circumstances (see question about overloading/overriding above).


* **When is a `static` block run?**</br>

     Code inside static block is executed only once: the first time you make an object of that class or the first time you access a static member of that class (even if you never make an object of that class).</br>
    Read more: [GeeksforGeeks](https://www.geeksforgeeks.org/g-fact-79/), [Video](https://study.com/academy/lesson/static-block-vs-constructor-in-java.html), [Beginnersbook](https://beginnersbook.com/2013/04/java-static-class-block-methods-variables/)


* **What is reflection?** [Jenkov](http://tutorials.jenkov.com/java-reflection/index.html), [GeeksforGeeks](https://www.geeksforgeeks.org/reflection-in-java/), [JavaTPoint](https://www.javatpoint.com/java-reflection), [Stackoverflow](https://stackoverflow.com/questions/37628/what-is-reflection-and-why-is-it-useful), [Baeldung](https://www.baeldung.com/java-reflection), [Guru99](https://www.guru99.com/java-reflection-api.html)</br>

    Java Reflection makes it possible to inspect classes, interfaces, fields and methods at runtime, without knowing the names of the classes, methods etc. at compile time. It is also possible to instantiate new objects, invoke methods and get/set field values using reflection.</br>


* **What is Dependency Injection?  Can you name few libraries? Have you used any?**
  - Dependency injection is a very powerful technique, where you relay the task of providing object with its' dependencies on instances of other objects (OOP Composition, [Wikipedia](https://en.wikipedia.org/wiki/Object_composition?oldformat=true)) to a separate class. This allows for fewer constructors, setters, factories and builders as all those functions are taken care of by the DI framework that you use. Also, and it may seem as a minor advantage, but if you use DI framework you need not worry about going through the project and changing all of (example names) `YourCustomInterface customInterfaceObject = new YourCustomClass();` to a new implementaion, as long as your new class (in place of `YourCustomClass`) still implements `CustomInterface` - you can just tweak the DI factory class to produce new class and voila - this new class will be automatically instantiated throughout your code. This allows for better maintenence and control over the program. Another example of DI usage is unit-testing - it allows to conveniently inject all needed dependencies and keep the amount of written code at a lower level.

  - One of the most popular libraries for DI for Android is Dagger 2. [MindOrks](https://blog.mindorks.com/a-complete-guide-to-learn-dagger-2-b4c7a570d99c), [Medium](https://medium.com/@harivigneshjayapalan/dagger-2-for-android-beginners-introduction-be6580cb3edb)

* **How is a `StringBuilder` implemented to avoid the immutable string allocation problem?** [Stackoverflow](https://stackoverflow.com/questions/54023816/how-is-a-stringbuilder-implemented-to-avoid-the-immutable-string-allocation-prob)


* **What is the difference between fail-fast and fail-safe iterators in Java?** [GeeksforGeeks](https://www.geeksforgeeks.org/fail-fast-fail-safe-iterators-java/)

  * Fail-fast Iterators throws ConcurrentModificationException when one Thread is iterating over collection object and other thread structurally modify Collection either by adding, removing or modifying objects on underlying collection. They are called fail-fast because they try to immediately throw Exception when they encounter failure.
  * On the other hand [fail-safe](http://javarevisited.blogspot.com/2011/10/java-iterator-tutorial-example-list.html) Iterators works on copy of collection instead of original collection.</br>


* **What is Java NIO?** [DZone](https://dzone.com/articles/java-nio-vs-io), [Baeldung](https://www.baeldung.com/java-nio-selector), [Howtodoinjava](https://howtodoinjava.com/java-nio-tutorials/)

* <b>Optionals in Java?</b></br>

    Optional is a container object which is used to contain not-null objects. Optional object is used to represent null with absent value. This class has various utility methods to facilitate code to handle values as ‘available’ or ‘not available’ instead of checking null values.</br>

  Read more: [Baeldung](https://www.baeldung.com/java-optional), [Mkyong](https://www.mkyong.com/java8/java-8-optional-in-depth/), [GeeksforGeeks](https://www.geeksforgeeks.org/java-8-optional-class/), [Callicoder](https://www.callicoder.com/java-8-optional-tutorial/)

* <b>What is externalization?</b></br>
   * In serialization, the JVM is responsible for the process of writing and reading objects. This is useful in most cases, as the programmers do not have to care about the underlying details of the serialization process.
   * However, the default serialization does not protect sensitive information such as passwords and credentials.
   * Thus externalization comes to give the programmers full control in reading and writing objects during serialization.
   * Implement the java.io.Externalizable interface - then you implement your own code to write object’s states in the ```writeExternal()``` method and read object’s states in the ```readExternal()``` method.</br>  
   Read more: [GeeksforGeeks](https://www.geeksforgeeks.org/externalizable-interface-java/), [CodeJava](https://www.codejava.net/java-se/file-io/understanding-java-externalization-with-examples)


* **Please explain Java annotation.** [Jaxenter](https://jaxenter.com/understand-annotations-java-148001.html), [Baeldung](https://www.baeldung.com/java-custom-annotation), [GeeksforGeeks](https://www.geeksforgeeks.org/annotations-in-java/), [JavaTPoint](https://www.javatpoint.com/java-annotation), [DZone](https://dzone.com/articles/how-annotations-work-java), [Jenkov](http://tutorials.jenkov.com/java/annotations.html)

* <b>Arrays in Java?</b></br>
   * Arrays is an ordered collection. It will have a fixed length which needs to be defined at the initialization time whereas lists have a variable length. Arrays are easier to store elements of the same data type. Used internally in stack and queue.    It is a convenient way of representing a 2D array.
   * Arrays cannot hold generic data types whereas lists can.
   * Arrays can store all data types whereas lists cannot store primitive data types, only objects.
   * Arrays: Complexity:

   	| Algorithm	|  Average	 | Worst Case  |
    | ---------- |:--------:| -----------:|
    | Space	    |	  Θ(n)		  |  O(n)       |
    | Search	   |   Θ(n)	   |  O(n)       |
    | Insert	   |   Θ(n)	   |  O(n)       |
    | Delete	   |   Θ(n)		  |  O(n)       |

    </br>


* <b>Linked Lists in Java?</b></br>
   * A LinkedList contains both a head and a tail. The "Head" is the first item in the LinkedList, while the "Tail" is the last item. It is not a circular data structure, therefore the tail does not have its' pointer pointing at the Head - the pointer is just null.
   * No indices but each node has a pointer pointing to the next element.
   * They are dynamic in nature which means they allocate memory only when needed.
   * Insertion, deletion, updation easy
   * A linked list is a group of nodes which represent a sequence. Each node consists of a data and a link or reference to the next node in the sequence.
   * <b>Singly Linked List</b>: has a node and a pointer to the next node in the sequence.
   * <b>Doubly Linked List</b>: has a node and 2 pointers - one to the next node and one to the previous node in the sequence. This is very convenient if you need to be able to traverse stored elements in both directions.
   * Linked List: Runtime Complexity:

   	| Algorithm	|  Average	 | Worst Case  |
    | ---------- |:--------:| -----------:|
    | Space	    |	  Θ(n)		  |  O(n)       |
    | Search	   |   Θ(n)	   |  O(n)       |
    | Insert	   |   Θ(1)	   |  O(1)       |
    | Delete	   |   Θ(1)		  |  O(1)       |

    </br>


* <b>Binary Tree</b></br>
   * A tree whose elements have at most 2 children is called a binary tree. Since each element in a binary tree can have only 2 children, we typically name them the left and right child.
   * The left subtree of a node contains only values less than the parent node's value.
   * The right subtree of a node contains only values greater than or equal to the node's value.
   * Only if the above 2 criteria are matched, then the tree is said to be balanced.
   * <b>Advantages of Binary tree over Linked List</b>: In a linked list, the items are linked together through a single next pointer. In a binary tree, as long as the tree is balanced, the searchpath to each item is a lot shorter than that in a linked list.
   * Their disadvantage is that in the worst case they can degenerate into a linked list in terms of efficiency.</br>



* <b>Stacks:</b></br>
   * Stacks are an abstract collection that follow LIFO mechanism.
   * Main functionalities include
       * <b>Push</b>: a new entity added to the top of the stack.
       * <b>Pop</b>: an entity is removed from the top of the stack.
   * The process of accessing data stored in a serial access memory is similar to manipulating data on a stack.
   * A stack may be defined to have a bounded capacity i.e. if the stack is full and a new entity cannot be added, then it is considered to be in an <b>overflow state</b>.
   * If the stack is empty and an entity cannot be popped, it is considered to be in an <b>underflow state</b>.
   * <b>Efficiency of stacks</b>: The time is not dependent of the no of items in the stack so it is very efficient. ```O(1)```.</br>



* <b>Queues:</b></br>
   * Queues are an abstract collection that follow FIFO mechanism. The entities in the queue are kept in an order.
   * Main functionalities include
       * <b>enqueue</b>: Add an item to the end of the queue. Dequeue: remove an item from the start of the queue.
       * <b>Front</b>: retrieves the first item from the queue.
   * A queue may be defined to have a bounded capacity i.e. if the queue is full and a new entity cannot be added, then it is considered to be in an <b>overflow state</b>.
   * If the queue is empty and an entity cannot be popped, it is considered to be in an <b>underflow state</b>.
   * <b>Efficiency of queues</b>: The time is not dependent of the no of items in the queue so it is very efficient. O(1).
   * <b>A double ended queue (deque)</b>: is an abstract collection which differs from queue in a way that an item can be added/removed from either side of the queue.
      * An <b>input-restricted deque</b>: is when deletion takes place at either end but insertion takes place at only one end.
      * An <b>output-restricted deque</b>: is when insertion takes place at either end but deletion takes place only at one end. A common occurrence of deque is doubly linked list.
   * <b>Priority queue</b>: same as queue but has a priority associated with it. Items are retrieved based on their priority</br>


* Java is unsound. Please explain. [Dev.to](https://dev.to/rosstate/java-is-unsound-the-industry-perspective)

* What is type erasure in Java? [Baeldung](https://www.baeldung.com/java-type-erasure), [GeeksforGeeks](https://www.geeksforgeeks.org/type-erasure-java/)

* <b>Difference between stacks & queues?</b></br>

    <a href="/image%20assets/stack-vs-queue.png"><img src="https://github.com/anitaa1990/Android-Cheat-sheet/blob/master/media/3.png"></a></br>   

</br>

* <b>What is a deadlock in Java</b></br>
   * A deadlock occurs when a thread enters a waiting state because a requested system resource is held by another waiting process, which in turn is waiting for another resource held by another waiting process.
   * [Example on how deadlock occurs](/src/deadlock/ThreadLockDemo.java)
   * [Example on how to prevent deadlock](/src/deadlock/ThreadLockFixedDemo.java)</br>



* <b>What is the List interface & Set interface?</b></br>
   * List interface supports for ordered collection of objects and it may contain duplicates. The Set interface provides methods for accessing the elements of a finite mathematical set. Sets do not allow duplicate elements</br>


* <b>Difference between ArrayList & Vectors?</b></br>
   * Vectors are thread safe (synchronized) whereas arraylists are not. So performance of arraylists are better than vectors.    * In ArrayList, you have to start searching for a particular element from the beginning of an Arraylist. But in the Vector, you can start searching for a particular element from a particular position in a vector. This makes the search operation in Vector faster than in ArrayList. Vectors have a default size of 10 whereas arraylists size can be dynamic.
   * <b>Insertion and deletion in ArrayList is slow compared to LinkedList?</b>
       * ArrayList internally uses an array to store the elements, when that array gets filled by inserting elements a new array of roughly 1.5 times the size of the original array is created and all the data of old array is copied to new array.
       * During deletion, all elements present in the array after the deleted elements have to be moved one step back to fill the space created by deletion. In linked list data is stored in nodes that have reference to the previous node and the next node so adding element is simple as creating the node and updating the next pointer on the last node and the previous pointer on the new node. Deletion in linked list is fast because it involves only updating the next pointer in the node before the deleted node and updating the previous pointer in the node after the deleted node.</br>      


* <b>Implementations of Map?</b></br>
   * <b>TreeMap</b>: sorted based on ascending order of keys. For inserting, deleting, and locating elements in a Map, the HashMap offers the best alternative. If, however, you need to traverse the keys in a sorted order, then TreeMap is your better alternative.
   *	<b>HashTable</b>: Does not allow null values. It is not fail-safe and it is synchronized whereas
   * <b>HashMap</b> allows null values and it is fail-safe and it is not synchronized.
   * <b>LinkedHashMap</b>: This is a subclass of Hashmap. The order of insertion is preserved since it has a linkedList.</br>


* <b>How Hashmap works in Java?</b></br>
   * HashMap in Java works on hashing principle. It is a data structure which allows us to store object and retrieve it in constant time O(1) provided we know the key. When we call put method, ```hashcode()``` method of the key object is called so that hash function of the map can find a bucket location to store Entry object.
   * If two different objects have the same hashcode: in this case, a linked list is formed at that bucket location and a new entry is stored as next node. After finding bucket location, we will call ```keys.equals()``` method to identify a correct node in LinkedList and return associated value object for that key in Java HashMap</br>



### Collection
* [30-seconds-of-java](https://github.com/iluwatar/30-seconds-of-java)
* [115 Java Interview Questions and Answers – The ULTIMATE List](http://www.javacodegeeks.com/2014/04/java-interview-questions-and-answers.html)
* [37 Java Interview Questions to Practice With from Codementor](https://www.codementor.io/java/tutorial/java-interview-sample-questions-answers)
* [21 Essential Java Interview Questions](http://www.toptal.com/java/interview-questions)
* [A collection of Java interview questions and answers to them The questions were gathered all around the Internet The answers are partly written by the commiters, partly copy-pasted from all possible sources](https://github.com/svozniuk/java-interviews)
* [There is the list of 201 core java interview questions The answers of the core java interview questions are short and to the point The core java interview questions are categorized in Basics of java interview questions, OOPs interview questions, String Handling interview questions, Multithreading interview questions, collection interview questions, JDBC interview questions etc](http://www.javatpoint.com/corejava-interview-questions)
* [Top 10 Tricky Java interview questions and Answers](http://java67.blogspot.com.by/2012/09/top-10-tricky-java-interview-questions-answers.html)
* [Top 25 Most Frequently Asked Interview Core Java Interview Questions And Answers](http://javahungry.blogspot.com/2013/06/top-25-most-frequently-asked-core-java.html)
* [Top 40 Core Java Interview Questions Answers from Telephonic Round](http://java67.blogspot.sg/2015/03/top-40-core-java-interview-questions-answers-telephonic-round.html)
* [Interview Cake Java Interview Questions](https://www.interviewcake.com/java-interview-questions)
* [Journaldev Core Java Interview Questions and Answers](https://www.journaldev.com/2366/core-java-interview-questions-and-answers)
* [Journaldev Java Exception Interview Questions and Answers](https://www.journaldev.com/2167/java-exception-interview-questions-and-answers)


### Read More

* [Snowdream - 115-Java-Interview-Questions](http://snowdream.github.io/115-Java-Interview-Questions-and-Answers/115-Java-Interview-Questions-and-Answers/en/index.html)

* [In28Minutes - Java Interview Questions And Answers](https://github.com/in28minutes/JavaInterviewQuestionsAndAnswers)
