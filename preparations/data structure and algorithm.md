## Contents

* [Problem Solving](#problem-solving)
* [Data structure](#data-structure)
* [Algorithm](#algorithm)
* [Collection](#collection)

### Problem Solving

> Basic problem solving of string, array, data manipulating etc.

## String

 - [GeeksForGeeks](https://www.geeksforgeeks.org/c-programs-gq/string-programs-gq/) - Around 30-40 Problems
 - [GeeksForGeeks Quiz](https://www.geeksforgeeks.org/c-string-question-9/) - Around 10-15 problems
 - [Aticleworld](https://aticleworld.com/string-interview-questions-in-c/) - around 20 problems
 - [w3resource](https://www.w3resource.com/c-programming-exercises/string/index.php) - 30 problems

## Array

* [Top 30 Array Interview Questions and Answers for Programmers](https://javarevisited.blogspot.com/2015/06/top-20-array-interview-questions-and-answers.html)


### Data Structure
* <b>What are Data Structures?</b></br>
   * Intentional arrangement of a collection of data. There are 5 fundamental behaviours of a data structure: access, insert, delete, find & sort.</br>


* <b>Explain Big O Notation?</b></br>
   * The notation Ο(n) is the formal way to express the upper bound of an algorithm's running time. It measures the worst case time complexity or the longest amount of time an algorithm can possibly take to complete.
   * Note: <b>O(1)</b> means that it takes a constant time, like three minutes no matter the amount of data in the set.
<b>O(n)</b> means it takes an amount of time linear with the size of the set.</br>


* <b>Explain Big Omega Notation</b></br>
   * The Big Omega Notation is used to describe the best case running time for a given algorithm.</br>

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


* <b>Blocking Queues:</b></br>
  * A blocking queue is a queue that blocks when you try to dequeue from it and the queue is empty, or if you try to enqueue items to it and the queue is already full. A thread trying to dequeue from an empty queue is blocked until some other thread inserts an item into the queue. A thread trying to enqueue an item in a full queue is blocked until some other thread makes space in the queue.
  * [Example on implementing a blocking queue](/src/queue/BlockingQueue.java)</br>

### Algorithm

### Collection
* 52 Programming Problems by Subeen.
 Solve the easiest problems from [here](https://dimikoj.com/problems).
* [Sherxon - AlgoDS](https://github.com/sherxon/AlgoDS)
