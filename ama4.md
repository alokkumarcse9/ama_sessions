### 1. What are `async` and `await`?

`async` is used to make a function asynchronous, and it always returns a Promise. `await` is used inside an async function to wait for a Promise to settle and get its result.

### 2. What is `console.log()`?

`console.log()` is a built-in JavaScript method used to print or display values in the console. It is mainly used for debugging and checking the output of our code.

### 3. What is the `typeof` of `null`?

The `typeof` of `null` is `"object"`. This is a historical behavior in JavaScript.

### 4. What is currying?

Currying is a technique where we convert a function that takes multiple arguments into multiple functions, where each function takes one argument at a time.

### 5. Explain `Promise.any()`.

`Promise.any()` is used when we have multiple Promises and want the result of the Promise that fulfills first. It ignores rejected Promises unless all Promises are rejected.

### 6. What is asynchronous programming?

Asynchronous programming means executing a task without blocking the execution of other code. JavaScript can start an asynchronous operation and continue executing other code while waiting for that operation to complete.

### 7. Why do we use `throw new Error()` instead of `try...catch`?

`throw new Error()` is used to create and raise an error, while `try...catch` is used to handle an error. They are not replacements for each other.

### 8. What is the difference between a function expression and a function declaration?

A function declaration is a function defined directly using the `function` keyword, while a function expression is a function stored inside a variable. Function declarations are hoisted, while function expressions are not hoisted.

### 9. How can we handle multiple promises and get the results even if some of them fail?

We can use `Promise.allSettled()` because it waits for all Promises to settle and returns the result of every Promise, whether it is fulfilled or rejected.

### 10. What is the difference between a `for...in` loop and a `for...of` loop?

`for...in` is used to iterate over the keys or indexes, while `for...of` is used to iterate over the values of an iterable.

### 11. What is the difference between `find()` and `filter()`?

`find()` returns the first element that satisfies the condition, while `filter()` returns all elements that satisfy the condition in an array.

### 12. What are Web APIs?

Web APIs are APIs provided by the browser that allow JavaScript to perform operations outside the JavaScript engine itself, such as timers, DOM manipulation, network requests, and browser-related tasks.

### 13. How do you convert an array of characters into a string?

We can use the `join()` method to convert an array of characters into a string.
