
Collections:

- [GitHub](https://github.com/sudheerj/javascript-interview-questions?tab=readme-ov-file#table-of-contents)
- [InterviewBit](https://www.interviewbit.com/javascript-interview-questions/)
- [Simplelearn](https://www.simplilearn.com/tutorials/javascript-tutorial/javascript-interview-questions)
- [roadmap.sh](https://roadmap.sh/questions/javascript)

### Design New

The questions that expose this gap:

1. Implement debounce function 
 - 90% get confused about closures and timers. 
 - This tests your understanding of scope, timing, and function composition.

2. Build your own Promise.all 
 - Most copy-paste from Stack Overflow without understanding async behavior. - Shows if you really know promises.

3. Create an Event Emitter class 
 - Tests object-oriented thinking, observer pattern, and memory management. - Many leak memory here.

4. Implement deep clone for objects 
 - Simple on surface, but handling circular references, different data types, and edge cases reveals true skill level.

5. Build getElementsByStyle function
 - Tests DOM traversal algorithms, CSS property matching, and performance considerations
 - Most struggle with recursive tree traversal and proper style computation
 - Reveals understanding of how browsers actually work under the hood

Why these matter: They're building blocks of every framework you use.

React hooks? Built on closures. 
State management? Event patterns. 
API optimization? Debounce and throttle.

Questions:

- **What are the different data types present in javascript?**
  - Primitive types: 
    - String:
      ```js
        vat str = "Hello world"
      ```
    - Number:
        ```js
        var x= 5;
        var y = 4.5;
        ```
    - BigInt:
        ```js
        var bigInteger = 8374034503745;
        ``` 
     - Boolean:
     ```js
     var hello = true;
     ```
    - Symbol: It is introduced in ES6 and used to store an anonymous and unique value.
    ```js
    var symbol1 = Symbol('Symbol');
    ```
  -Non-primitive types: Primitive types are used to store single value. But to store complex and multiple values, non-primitive data types are used.
  ```js
  var obj1 = {
    x:43,
    y:'Hello world',
    z: function(){
        return this.x;
    }
  }
    ```

- **Explain hoising in javascript.**
  - It is a default behaviour of javascript where all the variable and function **declarations** are moved on top. Like - 

    ```js
        hoistedVariable = 5;
        console.log(hoistedVariable); // output 5 even if it is declared at the end.
        var hoistedVariable;
    ```
    It works for function as well.
    ```js
    hoistedFunction(); //outputs Hello world!

    function hoistedFunction(){
        console.log("Hello world!");
    }
    ```
    Note 1 - Variable initializations are not hoisted only the declarations.
    ```js
    var x;
    console.log(x); // outputs undefined
    x=23;
    ```
    Note 2: To avoid hoisting, we can run javascript using `use strict` on top of the code.

- ** Why do we use the word “debugger” in javascript?**