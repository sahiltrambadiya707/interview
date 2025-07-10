Awesome! Below is the **full collection of logical JavaScript interview questions** — structured, deduplicated, categorized by **Topic** and **Difficulty** (🟢 Basic / 🟡 Mid / 🔴 Expert), and each includes the **expected output**.

---

## 🧠 JavaScript Logical & Tricky Interview Questions

---

### 🟢 BASIC LEVEL

---

#### 🔸 Type Coercion & Equality

```js
1 + "2" + "2"                 // "122"
1 + +"2" + "2"                // "32"
1 + -"1" + "2"                // "02"
+"1" + "1" + "2"              // "112"
typeof typeof 1              // "string"
2 + true                     // 3
Number(true)                 // 1
typeof null                  // "object"
typeof NaN                   // "number"
[] + []                      // ""
NaN === NaN                  // false
0.1 + 0.2 === 0.3            // false
[] == ![]                    // true
[] == 0                      // true
[null] == ''                 // true
[null] == 0                  // true
[undefined] == ''            // true
[undefined] == 0             // true
```

---

#### 🔸 Variable Basics & Hoisting

```js
console.log(a);
var a = 5;
// Output: undefined

console.log(employeeId);
var employeeId = '19000';
// Output: undefined
```

---

#### 🔸 Short-Circuit Logic

```js
console.log(null || "default");    // "default"
console.log("hello" && 123);       // 123
```

---

#### 🔸 Reference Behavior

```js
const a = [1, 2, 3];
const b = a;
b[0] = 99;
console.log(a); // [99, 2, 3]

const obj1 = { value: 10 };
const obj2 = obj1;
obj2.value = 20;
console.log(obj1); // { value: 20 }
```

---

#### 🔸 `this` Context

```js
const obj = {
  value: 42,
  getValue: function () {
    return this.value;
  }
};

console.log(obj.getValue()); // 42
console.log(obj.getValue.call({ value: 99 })); // 99
```

---

### 🟡 MID LEVEL

---

#### 🔸 Scoping & Execution Context

```js
var x = 10;
function foo() {
  console.log(x);
  var x = 20;
}
foo(); // undefined
```

```js
var a = 5;
(function () {
  console.log(a); // undefined
  var a = 10;
  console.log(a); // 10
})();
```

---

#### 🔸 Arrays & Sparse Assignment

```js
var a = [1, 2, 3];
a[10] = 10;
console.log(a.length); // 11
```

---

#### 🔸 Function Overriding & Hoisting

```js
function test() {
  console.log("test 1");
}
function test() {
  console.log("test 2");
}
test(); // "test 2"
```

```js
var greeting = function () {
  console.log("First greeting");
};
function greeting() {
  console.log("Second greeting");
}
greeting(); // First greeting
```

---

#### 🔸 Prototype & Inheritance

```js
function A() {}
A.prototype.x = 10;
const a = new A();
console.log(a.x); // 10
```

---

#### 🔸 Object Key Coercion

```js
const obj = {};
obj[true] = 'yes';
obj[1] = 'no';
console.log(obj[true]); // "no"
```

---

### 🔴 EXPERT LEVEL

---

#### 🔸 Async/Await & Event Loop

```js
async function asyncFunc() {
  console.log('A');
  await new Promise(resolve => setTimeout(resolve, 1000));
  console.log('B');
}
console.log('C');
asyncFunc();
console.log('D');
// Output: C, A, D, B
```

---

```js
console.log("Start");
setTimeout(() => console.log("Timeout"), 0);
Promise.resolve().then(() => console.log("Promise"));
console.log("End");
// Output: Start, End, Promise, Timeout
```

---

```js
console.log("1");
setTimeout(() => console.log("2"), 0);
Promise.resolve().then(() => console.log("3")).then(() => console.log("4"));
console.log("5");
// Output: 1, 5, 3, 4, 2
```

---

```js
console.log("1. Start");

process.nextTick(() => console.log("2. process.nextTick"));
Promise.resolve().then(() => console.log("3. Promise resolved"));
setTimeout(() => console.log("6. setTimeout with 0ms delay"), 0);
setImmediate(() => console.log("7. setImmediate"));

for (let i = 0; i < 1e9; i++) {}

console.log("4. Synchronous end");

// Output: 1. Start, 4. Synchronous end, 2..., 3..., 6..., 7...
```

---

#### 🔸 `let` vs `var` in Loops

```js
for (var i = 0; i < 4; i++) {
  setTimeout(() => console.log(i), 1000);
}
// Output: 4, 4, 4, 4

for (let i = 0; i < 4; i++) {
  setTimeout(() => console.log(i), 1000);
}
// Output: 0, 1, 2, 3
```

---

```js
const b = [1,2,3,4,5,6,7,8,9,10];

for (let i = 0; i < 10; i++) {
  setTimeout(() => console.log(b[i]), 1000); // 0 to 9
}

for (var i = 0; i < 10; i++) {
  setTimeout(() => console.log(b[i]), 1000); // undefined printed 10 times
}
```

---

#### 🔸 TDZ (Temporal Dead Zone)

```js
console.log(x);
let x = 5;
// ReferenceError: Cannot access 'x' before initialization
```

---

#### 🔸 Promise + Microtasks + Macrotasks

```js
console.log('Start');
Promise.resolve().then(() => console.log('Promise 1'));
setTimeout(() => console.log('Timeout 1'), 0);
Promise.resolve().then(() => console.log('Promise 2'));
setTimeout(() => console.log('Timeout 2'), 0);
console.log('End');

// Output: Start, End, Promise 1, Promise 2, Timeout 1, Timeout 2
```

---

# 🧠 Logical JavaScript Interview Questions (50+)

Each question is grouped by topic and marked with a difficulty tag:

* 🟢 Basic
* 🟡 Mid
* 🔴 Expert

---

## 🔸 Type Coercion & Comparison

| Difficulty | Code                      | Output                       |
| ---------- | ------------------------- | ---------------------------- |
| 🟢         | `1 + "2" + "2"`           | `"122"`                      |
| 🟢         | `1 + +"2" + "2"`          | `"32"`                       |
| 🟢         | `1 + -"1" + "2"`          | `"02"`                       |
| 🟢         | `+"1" + "1" + "2"`        | `"112"`                      |
| 🟢         | `typeof typeof 1`         | `"string"`                   |
| 🟢         | `2 + true`                | `3`                          |
| 🟢         | `[] == ![]`               | `true`                       |
| 🟢         | `NaN === NaN`             | `false`                      |
| 🟢         | `[1, 2, 3] + [4, 5, 6]`   | `"1,2,34,5,6"`               |
| 🟢         | `typeof null`             | `"object"`                   |
| 🟢         | `typeof NaN === "number"` | `true`                       |
| 🟢         | `[] + []`                 | `""`                         |
| 🟢         | `0.1 + 0.2 === 0.3`       | `false`                      |
| 🟢         | `[null] == ''`            | `true`                       |
| 🟢         | `[null] == 0`             | `true`                       |
| 🟢         | `[undefined] == ''`       | `true`                       |
| 🟢         | `[undefined] == 0`        | `true`                       |
| 🟡         | `[1] == true`             | `true`                       |
| 🟡         | `[1,2] == "1,2"`          | `true`                       |
| 🔴         | `{ } + []`                | `0` (depends on environment) |

---

## 🔸 Hoisting & Variable Scope

| Difficulty | Code                                                               | Output           |
| ---------- | ------------------------------------------------------------------ | ---------------- |
| 🟢         | `console.log(a); var a = 5;`                                       | `undefined`      |
| 🟢         | `console.log(employeeId); var employeeId = '19000';`               | `undefined`      |
| 🟡         | `var x = 10; function foo(){ var x = 20; console.log(x); } foo();` | `20`             |
| 🔴         | `var x = 10; function foo(){ console.log(x); var x = 20; } foo();` | `undefined`      |
| 🔴         | `console.log(a); let a = 5;`                                       | `ReferenceError` |
| 🟡         | `var a = 5; (function() { console.log(a); var a = 10; })();`       | `undefined`      |

---

## 🔸 Functions & Overriding

| Difficulty | Code                                                                          | Output              |
| ---------- | ----------------------------------------------------------------------------- | ------------------- |
| 🟡         | Function redeclaration → `function test() {}` (twice) then call `test()`      | last one overrides  |
| 🟡         | Hoisting → `greeting(); var greeting = function() {...}`                      | `TypeError`         |
| 🟡         | `console.log(test()); function test() {...}` vs arrow function version        | behaves differently |
| 🔴         | Named vs anonymous function `const fn = function() {}; console.log(fn.name);` | `fn`                |

---

## 🔸 Async/Await & Event Loop

| Difficulty | Code                                                                  | Output                          |
| ---------- | --------------------------------------------------------------------- | ------------------------------- |
| 🟡         | `console.log('Start'); setTimeout(...); Promise.resolve().then(...);` | Start, End, Promise, Timeout    |
| 🔴         | `async function(){ await ... }` interleaved with sync and async logs  | mixed order                     |
| 🔴         | `process.nextTick(...)`, `setTimeout(...)`, `setImmediate(...)`       | nextTick > Promise > setTimeout |
| 🔴         | Multiple `.then()` chained vs parallel                                | microtask queuing               |

---

## 🔸 Loops & Closures

| Difficulty | Code                                                                 | Output                                  |
| ---------- | -------------------------------------------------------------------- | --------------------------------------- |
| 🟢         | `for (let i=0; i<4; i++) { setTimeout(() => console.log(i)); }`      | 0 1 2 3                                 |
| 🟡         | `for (var i=0; i<4; i++) { setTimeout(() => console.log(i)); }`      | 4 4 4 4                                 |
| 🔴         | `const b = [1,2,3...];` loop with `let` vs `var` inside `setTimeout` | `let` = index values, `var` = undefined |

---

## 🔸 Objects & References

| Difficulty | Code                                                              | Output               |
| ---------- | ----------------------------------------------------------------- | -------------------- |
| 🟢         | `const arrA = [0,1]; const arrB = arrA; arrB[0] = 99;`            | `[99, 1]`            |
| 🟢         | `var objA = {x: 10}; var objB = objA; objB.x = 20;`               | `{x: 20}`            |
| 🔴         | `Object.freeze({inner: {a: 1}}).inner.a = 2`                      | `2` (shallow freeze) |
| 🔴         | `const obj = {}; obj[true] = 'yes'; obj[1] = 'no';` → `obj[true]` | `"no"`               |

---

## 🔸 Prototype & Inheritance

| Difficulty | Code                                                                                 | Output         |
| ---------- | ------------------------------------------------------------------------------------ | -------------- |
| 🟡         | `function A(){}; A.prototype.x = 10; const a = new A(); console.log(a.x);`           | `10`           |
| 🔴         | `Foo.prototype = {x:1}; const f = new Foo(); Foo.prototype.x = 2; console.log(f.x);` | `2` (live ref) |

---

## 🔸 Advanced Topics

| Difficulty | Code                                                       | Output                                              |
| ---------- | ---------------------------------------------------------- | --------------------------------------------------- |
| 🔴         | Proxy trap example intercepting `get`                      | `"intercepted"`                                     |
| 🔴         | WeakMap GC → `obj = null`                                  | entry GC-ed                                         |
| 🔴         | `JSON.stringify` with circular refs                        | crashes without replacer                            |
| 🔴         | Tagged template literals                                   | `tag\`Hello \${1 + 2}\``→`\["Hello ", ""]`, `\[3]\` |
| 🔴         | Destructured default values: `function fn({a=1} = {a: 3})` | varies by param                                     |
| 🔴         | Generator with async iteration                             | works with `for await`                              |
| 🔴         | Trampoline functions for deep recursion                    | stack-safe                                          |
| 🔴         | Array sort + Math.random()                                 | not stable                                          |
| 🔴         | `Symbol` vs string keys                                    | different behavior                                  |
| 🔴         | `Object.freeze`, `seal`, `preventExtensions` differences   | mutate vs block                                     |

---

