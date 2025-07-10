---

### ✅ FORMAT:

Each section is grouped by:

* **Technology**
* **Difficulty Level (Basic / Mid / Expert)**
* **Well-formatted questions**

---

## ⚛️ REACT.js

---

### 🟢 Basic

1. What is React and how does it differ from vanilla JavaScript?
2. What are components in React?
3. What is the difference between a functional and class component?
4. What is JSX and why do we use it?
5. How do you pass data between components in React?
6. What are props and how are they different from state?
7. How do you handle events in React?
8. What is the purpose of `key` in a list?
9. What happens when you call `setState`?
10. How do you conditionally render elements in React?

---

### 🟡 Mid

1. What problems does React solve that traditional JavaScript struggles with?
2. Why is React considered declarative? Provide an example.
3. Explain the rules of hooks — why do they exist?
4. What is the difference between Controlled and Uncontrolled components? When to use which?
5. How does React’s `StrictMode` help with code quality?
6. How do you lazy load components and handle fallback states?
7. Why should keys be stable and unique in lists? Why are indexes discouraged?
8. How does `useEffect` work, and how can dependency arrays impact performance?
9. Explain the difference between `useEffect`, `useLayoutEffect`, and `useInsertionEffect`.

---

### 🔴 Expert

1. Explain how React reconciles the Virtual DOM with the actual DOM.
2. How does React batch state updates, and how can that impact performance?
3. When would you use `useCallback` vs `useMemo`? Give a performance scenario.
4. How does `useReducer` compare to Redux in managing local component state?
5. Explain stale closures in `useEffect` and how to avoid related bugs.
6. What are custom hooks and how do they improve code reuse?
7. How would you memoize an entire component tree to prevent unnecessary renders?
8. Describe Context API. How does it compare to Redux?
9. Explain Render Props vs HOC vs Custom Hook.
10. How do you solve deep prop drilling without Context or Redux?
11. What is code-splitting? How does it affect Time to Interactive?
12. How can you prevent XSS in React? What about CSRF?
13. How do you implement route guards in React Router v6?
14. In Redux, how do you handle side-effects with middleware like thunk or saga?
15. How would you implement optimistic UI updates with Redux?

---

## 🟨 JavaScript

---

### 🟢 Basic

1. What are the different data types in JavaScript?
2. What is the difference between `var`, `let`, and `const`?
3. What is hoisting in JavaScript?
4. What is a function and how do you declare one?
5. What is the difference between `==` and `===`?
6. What are arrays and objects in JS?
7. How do you clone an object?
8. How do you check if a variable is an array?
9. What are arrow functions and how do they differ from regular functions?
10. What is `this` keyword in JS?

---

### 🟡 Mid

1. Explain event delegation with an example use-case.
2. What is the Temporal Dead Zone and how does it apply to `let` and `const`?
3. What are closures and how do they work?
4. Explain currying with a real-world use case.
5. Compare function expressions, declarations, and arrow functions in terms of `this`.
6. Describe debouncing vs throttling. When would you use each?
7. How does JavaScript handle garbage collection?
8. What is the use of `Symbol` in JS?
9. How is prototypal inheritance different from classical inheritance?
10. What are `map`, `filter`, and `reduce` and when would you use them?

---

### 🔴 Expert

1. What is the difference between microtasks and macrotasks? Where does `Promise.then` fit?
2. Write a polyfill for `Promise.allSettled`.
3. What is a race condition? How do you prevent it in async JavaScript?
4. How does `async/await` work under the hood?
5. What is a trampoline function and why would you use it?
6. What is the difference between `Object.freeze`, `Object.seal`, and `Object.preventExtensions`?
7. How do service workers improve performance?
8. Why can't web workers access the DOM? How do you use them safely?
9. How do you securely store JWT tokens in the browser?
10. How does the event loop work with `setTimeout`, `Promise`, and `async/await`?

---

## 🌐 Node.js

---

### 🟢 Basic

1. What is Node.js and why is it used?
2. How is Node.js different from traditional backend frameworks?
3. What is NPM and how do you use it?
4. How do you read/write files using Node.js?
5. What is the use of `require` in Node?
6. What is the difference between `module.exports` and `exports`?
7. How do you create a basic HTTP server in Node?
8. What are environment variables and how do you access them?

---

### 🟡 Mid

1. Explain the event loop in Node.js.
2. What is `libuv` and what role does it play in Node?
3. What are worker threads vs child processes?
4. When to use `cluster` vs `worker_threads`?
5. How does Express middleware chaining work?
6. How is the `Buffer` class used and how does it differ from Array?
7. What is streaming in Node.js? Why is it important?
8. What is the difference between synchronous and asynchronous file operations?
9. How do you secure Express APIs?

---

### 🔴 Expert

1. How would you handle long-running CPU-bound operations in Node.js?
2. How to build a rate limiter in Node.js?
3. How would you implement in-memory caching in Node?
4. What are some strategies to scale Node.js in a production environment?
5. How to ensure graceful shutdown and cleanup of open connections?
6. How do you handle circular dependency issues in Node modules?
7. How would you monitor and trace memory leaks in Node.js?

---

## 🚀 MongoDB

---

### 🟢 Basic

1. What is MongoDB and how is it different from SQL databases?
2. What is a collection and a document in MongoDB?
3. What is the `_id` field and how is it generated?
4. How do you insert, update, delete documents in MongoDB?
5. What is BSON?
6. What are the common data types supported in MongoDB?

---

### 🟡 Mid

1. Compare SQL vs NoSQL schema design (e.g. eCommerce app).
2. What is indexing in MongoDB? How does it improve performance?
3. What are compound indexes and when would you use them?
4. What is document-level atomicity?
5. Write a query to group orders by user and calculate total.
6. What is the difference between `find`, `aggregate`, and `distinct`?
7. What is `$match` vs `$project` in an aggregation pipeline?

---

### 🔴 Expert

1. Explain `$facet`, `$bucket`, and `$densify` with examples.
2. What is the difference between `$lookup` and `$graphLookup`?
3. How do you implement full-text search and fallback to regex search?
4. What are write concerns and read preferences? How do they affect consistency?
5. How does sharding work? What are the tradeoffs?
6. How would you handle slow queries and optimize them?
7. How would you enforce unique constraints across multiple fields?

---

## 🙋 Behavioral

(All questions below are **all levels** — useful for screening soft skills.)

1. Tell me about a time you faced a technical failure. What did you learn?
2. Have you disagreed with a teammate? How did you handle it?
3. What’s a technical decision you made that turned out well or poorly?
4. How do you balance writing clean code and delivering on time?
5. How do you handle feedback, especially critical code reviews?
6. How do you approach learning a new technology under a deadline?
7. What excites you most about this role?

---
