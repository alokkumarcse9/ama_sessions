# AMA Questions and Answers

### 1. What is `finally()`?

`finally()` is used with a Promise. It runs after the Promise is completed, whether it is resolved or rejected.

```javascript
promise
    .then(() => {
        console.log("Success");
    })
    .catch(() => {
        console.log("Error");
    })
    .finally(() => {
        console.log("Done");
    });
```



### 2. What are synchronous and asynchronous operations in JavaScript?

**Synchronous:** Code runs one by one and waits for each operation to finish.

```javascript
console.log("A");
console.log("B");
console.log("C");
```

**Asynchronous:** Code can continue running without waiting for an operation to finish.

```javascript
console.log("A");

setTimeout(() => {
    console.log("B");
}, 1000);

console.log("C");
```

Output:

```text
A
C
B
```

### 3. What is the `GROUP BY` clause in SQL?

`GROUP BY` is used to group rows with the same value.

### 4. In HTML, what happens if we use `<>` without specifying a tag name?

`<>` is not a valid HTML tag by itself.

A tag should have a tag name, for example:

```html
<div>Hello</div>
```

So, `<>` without a tag name is invalid HTML.

### 5. In Git, if we make a commit and want to add changes to the previous commit, how can we do it?

We can use `git commit --amend`.



### 6. What is `JSON.parse()`?

`JSON.parse()` converts a JSON string into a JavaScript object.

```javascript
const data = '{"name":"Alok","age":22}';

const user = JSON.parse(data);

console.log(user.name);
```

Output:

```text
Alok
```


### 7. Why do we use `box-sizing` in CSS?

`box-sizing` controls how the width and height of an element are calculated.

A common approach is:

```css
* {
    box-sizing: border-box;
}
```

With `border-box`, the width includes the content, padding, and border.

### 8. How do you remove an element from the DOM?

We can use the `remove()` method.

```javascript
const element = document.querySelector("#box");

element.remove();
```


### 9. What is the DOM?

DOM stands for **Document Object Model**.

The browser converts HTML into a **tree-like structure of objects**.

JavaScript uses the DOM to:

* Select elements
* Change content
* Change styles
* Add elements
* Remove elements
* Handle events


### 10. What is event bubbling?

Event bubbling means an event starts from the target element and moves upward to its parent elements.

For example:

```text
Button → Div → Body → HTML → Document
```

This process is called **event bubbling**.


### 11. What is `setTimeout()`?

`setTimeout()` is used to run a function **after a specified amount of time**.

```javascript
setTimeout(() => {
    console.log("Hello");
}, 2000);
```

Here, the function runs after approximately 2 seconds.

### 12. Why should we not use `forEach()` with `async/await`?

`forEach()` does not wait for the `async` callback to finish.

Instead, when we want to wait for each operation, we can use `for...of`.

```javascript
for (const item of items) {
    await processItem(item);
}
```

`for...of` waits for each `await` before moving to the next item.


### 13. Which HTTP method is used to create new data?

The **POST** method is generally used to create new data.

Example:

```http
POST /users
```

It sends new data to the server.
