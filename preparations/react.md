### Questions

1. What are the limitations of React in building large-scale applications?

2. How does React manage the Virtual DOM, and what are the benefits?

3. Can React Hooks fully replace Redux for state management? Explain why or why not.

4. What are the best practices for managing state in large React applications?

5. How would you optimize performance in a React app with large component trees?

6. Explain React's Strict Mode and its impact on development.

7. How can you prevent unnecessary re-renders in React functional components?

8. Describe the key differences between functional and class components in React.

9. What is the significance of the React Fiber architecture?

10. How does React handle side effects, and how can you manage them effectively?

11. Explain the differences between `useMemo()` and `useCallback()` in React.

12. How would you implement dynamic form handling and validation in React?

13. What is lazy loading in React, and how does it improve application performance?

14. How would you handle errors in a React app, and what is the role of error boundaries?

15. What are the benefits of server-side rendering (SSR) in React applications?

16. How do you handle styling in React components? Discuss different approaches.

17. How would you pass data between sibling components in React without using Redux?

18. Explain the use case of `useEffect()` for fetching data from an API.

19. How do you handle asynchronous operations in React using `async/await` or Promises?

20. How would you re-render a component when the window is resized?

21. Describe how React Context API can be used for state management in an app.

22. What is the role of React Router, and how does it work with dynamic routing?

23. Explain the concept of controlled and uncontrolled components in React.

24. How would you optimize React app performance when handling large lists or grids?

25. Explain the difference between shallow and deep comparison in React's `shouldComponentUpdate`.

26. How do you handle asynchronous code execution and state updates in React?

27. How would you implement custom hooks to abstract logic in React?

28. What are higher-order components (HOCs) in React, and how are they used?

29. How would you implement a search feature with debouncing in React?

30. Explain React's reconciliation process and how it updates the DOM efficiently.

---------
---------

𝗔𝗿𝗰𝗵𝗶𝘁𝗲𝗰𝘁𝘂𝗿𝗲 & 𝗖𝗼𝗿𝗲 𝗖𝗼𝗻𝗰𝗲𝗽𝘁𝘀
1. 𝘞𝘩𝘢𝘵 𝘢𝘳𝘦 𝘵𝘩𝘦 𝘭𝘪𝘮𝘪𝘵𝘢𝘵𝘪𝘰𝘯𝘴 𝘰𝘧 𝘙𝘦𝘢𝘤𝘵 𝘪𝘯 𝘭𝘢𝘳𝘨𝘦-𝘴𝘤𝘢𝘭𝘦 𝘢𝘱𝘱𝘴?
2. 𝘏𝘰𝘸 𝘥𝘰𝘦𝘴 𝘵𝘩𝘦 𝘝𝘪𝘳𝘵𝘶𝘢𝘭 𝘋𝘖𝘔 𝘸𝘰𝘳𝘬 𝘪𝘯 𝘙𝘦𝘢𝘤𝘵, 𝘢𝘯𝘥 𝘸𝘩𝘺 𝘥𝘰𝘦𝘴 𝘪𝘵 𝘮𝘢𝘵𝘵𝘦𝘳?
3. 𝘊𝘢𝘯 𝘙𝘦𝘢𝘤𝘵 𝘏𝘰𝘰𝘬𝘴 𝘳𝘦𝘱𝘭𝘢𝘤𝘦 𝘙𝘦𝘥𝘶𝘹? 𝘞𝘩𝘺 𝘰𝘳 𝘸𝘩𝘺 𝘯𝘰𝘵?
4. 𝘉𝘦𝘴𝘵 𝘱𝘳𝘢𝘤𝘵𝘪𝘤𝘦𝘴 𝘧𝘰𝘳 𝘮𝘢𝘯𝘢𝘨𝘪𝘯𝘨 𝘴𝘵𝘢𝘵𝘦 𝘢𝘵 𝘴𝘤𝘢𝘭𝘦?
5. 𝘗𝘦𝘳𝘧𝘰𝘳𝘮𝘢𝘯𝘤𝘦 𝘰𝘱𝘵𝘪𝘮𝘪𝘻𝘢𝘵𝘪𝘰𝘯 𝘪𝘯 𝘢𝘱𝘱𝘴 𝘸𝘪𝘵𝘩 𝘥𝘦𝘦𝘱 𝘤𝘰𝘮𝘱𝘰𝘯𝘦𝘯𝘵 𝘵𝘳𝘦𝘦𝘴?
6. 𝘞𝘩𝘢𝘵'𝘴 𝘙𝘦𝘢𝘤𝘵 𝘚𝘵𝘳𝘪𝘤𝘵 𝘔𝘰𝘥𝘦 𝘢𝘯𝘥 𝘸𝘩𝘺 𝘴𝘩𝘰𝘶𝘭𝘥 𝘺𝘰𝘶 𝘤𝘢𝘳𝘦?

𝗥𝗲-𝗿𝗲𝗻𝗱𝗲𝗿𝘀 & 𝗛𝗼𝗼𝗸𝘀 𝗠𝗮𝘀𝘁𝗲𝗿𝘆 
7. 𝘏𝘰𝘸 𝘵𝘰 𝘱𝘳𝘦𝘷𝘦𝘯𝘵 𝘶𝘯𝘯𝘦𝘤𝘦𝘴𝘴𝘢𝘳𝘺 𝘳𝘦-𝘳𝘦𝘯𝘥𝘦𝘳𝘴 𝘪𝘯 𝘧𝘶𝘯𝘤𝘵𝘪𝘰𝘯𝘢𝘭 𝘤𝘰𝘮𝘱𝘰𝘯𝘦𝘯𝘵𝘴?
 8. 𝘒𝘦𝘺 𝘥𝘪𝘧𝘧𝘦𝘳𝘦𝘯𝘤𝘦𝘴: 𝘧𝘶𝘯𝘤𝘵𝘪𝘰𝘯𝘢𝘭 𝘷𝘴 𝘤𝘭𝘢𝘴𝘴 𝘤𝘰𝘮𝘱𝘰𝘯𝘦𝘯𝘵𝘴?
 9. 𝘞𝘩𝘺 𝘪𝘴 𝘙𝘦𝘢𝘤𝘵 𝘍𝘪𝘣𝘦𝘳 𝘪𝘮𝘱𝘰𝘳𝘵𝘢𝘯𝘵? 
10. 𝘔𝘢𝘯𝘢𝘨𝘪𝘯𝘨 𝘴𝘪𝘥𝘦 𝘦𝘧𝘧𝘦𝘤𝘵𝘴 𝘵𝘩𝘦 𝘳𝘪𝘨𝘩𝘵 𝘸𝘢𝘺
 11. 𝘶𝘴𝘦𝘔𝘦𝘮𝘰() 𝘷𝘴 𝘶𝘴𝘦𝘊𝘢𝘭𝘭𝘣𝘢𝘤𝘬() – 𝘳𝘦𝘢𝘭 𝘶𝘴𝘦 𝘤𝘢𝘴𝘦𝘴

𝗙𝗼𝗿𝗺𝘀, 𝗘𝗳𝗳𝗲𝗰𝘁𝘀 & 𝗔𝘀𝘆𝗻𝗰 𝗟𝗼𝗴𝗶𝗰 
12. 𝘏𝘢𝘯𝘥𝘭𝘪𝘯𝘨 𝘥𝘺𝘯𝘢𝘮𝘪𝘤 𝘧𝘰𝘳𝘮𝘴 + 𝘷𝘢𝘭𝘪𝘥𝘢𝘵𝘪𝘰𝘯? 
13. 𝘓𝘢𝘻𝘺 𝘭𝘰𝘢𝘥𝘪𝘯𝘨 𝘪𝘯 𝘙𝘦𝘢𝘤𝘵 – 𝘸𝘩𝘦𝘯 & 𝘸𝘩𝘺
14. 𝘌𝘳𝘳𝘰𝘳 𝘣𝘰𝘶𝘯𝘥𝘢𝘳𝘪𝘦𝘴 + 𝘨𝘳𝘢𝘤𝘦𝘧𝘶𝘭 𝘦𝘳𝘳𝘰𝘳 𝘩𝘢𝘯𝘥𝘭𝘪𝘯𝘨 
15. 𝘚𝘚𝘙 𝘣𝘦𝘯𝘦𝘧𝘪𝘵𝘴 𝘢𝘯𝘥 𝘵𝘳𝘢𝘥𝘦-𝘰𝘧𝘧𝘴
16. 𝘚𝘵𝘺𝘭𝘪𝘯𝘨 𝘢𝘱𝘱𝘳𝘰𝘢𝘤𝘩𝘦𝘴 𝘪𝘯 𝘙𝘦𝘢𝘤𝘵 – 𝘊𝘚𝘚 𝘔𝘰𝘥𝘶𝘭𝘦𝘴, 𝘚𝘵𝘺𝘭𝘦𝘥 𝘊𝘰𝘮𝘱𝘰𝘯𝘦𝘯𝘵𝘴, 𝘦𝘵𝘤. 
17. 𝘗𝘢𝘴𝘴𝘪𝘯𝘨 𝘥𝘢𝘵𝘢 𝘣𝘦𝘵𝘸𝘦𝘦𝘯 𝘴𝘪𝘣𝘭𝘪𝘯𝘨𝘴 𝘸𝘪𝘵𝘩𝘰𝘶𝘵 𝘙𝘦𝘥𝘶𝘹

𝗗𝗮𝘁𝗮 𝗙𝗲𝘁𝗰𝗵𝗶𝗻𝗴 & 𝗥𝗼𝘂𝘁𝗶𝗻𝗴 
18. 𝘜𝘴𝘪𝘯𝘨 𝘶𝘴𝘦𝘌𝘧𝘧𝘦𝘤𝘵() 𝘵𝘰 𝘧𝘦𝘵𝘤𝘩 𝘈𝘗𝘐 𝘥𝘢𝘵𝘢 
19. 𝘏𝘢𝘯𝘥𝘭𝘪𝘯𝘨 𝘢𝘴𝘺𝘯𝘤 𝘰𝘱𝘦𝘳𝘢𝘵𝘪𝘰𝘯𝘴 𝘶𝘴𝘪𝘯𝘨 𝘢𝘴𝘺𝘯𝘤/𝘢𝘸𝘢𝘪𝘵 
20. 𝘞𝘪𝘯𝘥𝘰𝘸 𝘳𝘦𝘴𝘪𝘻𝘦 𝘩𝘢𝘯𝘥𝘭𝘪𝘯𝘨 𝘢𝘯𝘥 𝘳𝘦-𝘳𝘦𝘯𝘥𝘦𝘳𝘴 
21. 𝘞𝘩𝘦𝘯 & 𝘩𝘰𝘸 𝘵𝘰 𝘶𝘴𝘦 𝘊𝘰𝘯𝘵𝘦𝘹𝘵 𝘈𝘗𝘐 𝘧𝘰𝘳 𝘴𝘵𝘢𝘵𝘦 
22. 𝘏𝘰𝘸 𝘙𝘦𝘢𝘤𝘵 𝘙𝘰𝘶𝘵𝘦𝘳 𝘩𝘢𝘯𝘥𝘭𝘦𝘴 𝘥𝘺𝘯𝘢𝘮𝘪𝘤 𝘳𝘰𝘶𝘵𝘦𝘴?

𝗔𝗱𝘃𝗮𝗻𝗰𝗲𝗱 𝗣𝗮𝘁𝘁𝗲𝗿𝗻𝘀 
23. 𝘊𝘰𝘯𝘵𝘳𝘰𝘭𝘭𝘦𝘥 𝘷𝘴 𝘶𝘯𝘤𝘰𝘯𝘵𝘳𝘰𝘭𝘭𝘦𝘥 𝘤𝘰𝘮𝘱𝘰𝘯𝘦𝘯𝘵𝘴 
24. 𝘖𝘱𝘵𝘪𝘮𝘪𝘻𝘪𝘯𝘨 𝘱𝘦𝘳𝘧𝘰𝘳𝘮𝘢𝘯𝘤𝘦 𝘧𝘰𝘳 𝘭𝘢𝘳𝘨𝘦 𝘭𝘪𝘴𝘵𝘴/𝘨𝘳𝘪𝘥𝘴 
25. 𝘚𝘩𝘢𝘭𝘭𝘰𝘸 𝘷𝘴 𝘥𝘦𝘦𝘱 𝘤𝘰𝘮𝘱𝘢𝘳𝘪𝘴𝘰𝘯 𝘪𝘯 𝘴𝘩𝘰𝘶𝘭𝘥𝘊𝘰𝘮𝘱𝘰𝘯𝘦𝘯𝘵𝘜𝘱𝘥𝘢𝘵𝘦() 26. 𝘈𝘴𝘺𝘯𝘤 𝘤𝘰𝘥𝘦 𝘦𝘹𝘦𝘤𝘶𝘵𝘪𝘰𝘯 + 𝘴𝘵𝘢𝘵𝘦 𝘶𝘱𝘥𝘢𝘵𝘦 𝘱𝘢𝘵𝘵𝘦𝘳𝘯𝘴 
27. 𝘊𝘳𝘦𝘢𝘵𝘪𝘯𝘨 𝘢𝘯𝘥 𝘶𝘴𝘪𝘯𝘨 𝘤𝘶𝘴𝘵𝘰𝘮 𝘩𝘰𝘰𝘬𝘴 
28. 𝘞𝘩𝘢𝘵 𝘢𝘳𝘦 𝘏𝘖𝘊𝘴 (𝘏𝘪𝘨𝘩𝘦𝘳-𝘖𝘳𝘥𝘦𝘳 𝘊𝘰𝘮𝘱𝘰𝘯𝘦𝘯𝘵𝘴)? 
29. 𝘋𝘦𝘣𝘰𝘶𝘯𝘤𝘦𝘥 𝘴𝘦𝘢𝘳𝘤𝘩 – 𝘩𝘰𝘸 𝘸𝘰𝘶𝘭𝘥 𝘺𝘰𝘶 𝘣𝘶𝘪𝘭𝘥 𝘪𝘵? 
30. 𝘙𝘦𝘢𝘤𝘵'𝘴 𝘳𝘦𝘤𝘰𝘯𝘤𝘪𝘭𝘪𝘢𝘵𝘪𝘰𝘯 𝘱𝘳𝘰𝘤𝘦𝘴𝘴 𝘪𝘯 𝘴𝘪𝘮𝘱𝘭𝘦 𝘵𝘦𝘳𝘮𝘴

----------
----------

𝗘𝘀𝘀𝗲𝗻𝘁𝗶𝗮𝗹 𝗥𝗲𝗮𝗰𝘁 𝗜𝗻𝘁𝗲𝗿𝘃𝗶𝗲𝘄 𝗤𝘂𝗲𝘀𝘁𝗶𝗼𝗻𝘀
1. What is the difference between React Node, Element, and Component?
2. What are React Fragments used for?
3. What is the purpose of the key prop in React?
4. What is the consequence of using array indices as keys?
5. What is the difference between Controlled and Uncontrolled components?
6. How would you lift state up and why is it necessary?
7. What are Pure Components?
8. What is the difference between createElement and cloneElement?
9. What is the role of PropTypes in React?
10. What are stateless components?
11. What are stateful components?
12. What are the benefits of using hooks in React?
13. What are the rules of React hooks?
14. What is the difference between useEffect and useLayoutEffect?
15. What does the dependency array of useEffect affect?
16. What is the useRef hook and when should it be used?
17. Why does React recommend against mutating state?
18. What is reconciliation in React?
19. What is hydration in React?
20. Explain higher-order components (HOCs)
21. What are some common performance optimization techniques in React?
22. What is the purpose of the useReducer hook in React?
23. How do you test a React application?
24. What is server-side rendering (SSR)?
25. What is Static site generation (SSG)?
26. What is lazy loading in React?
27. What is the purpose of the useContext hook in React?
28. What is the purpose of the useMemo hook in React?
29. What is the purpose of the useCallback hook in React?
30. What is the purpose of the useImperativeHandle hook in React?