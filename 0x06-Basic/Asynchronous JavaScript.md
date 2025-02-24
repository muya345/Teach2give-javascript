# Asynchronous JavaScript
It refers to the execution of JavaScript without blocking the main thread, allowing other operations to continue while waiting for other tasks to complete.


In JavaScript, asynchronous programming is done using Promises.

Example of what asynchronous JavaScript looks like:
```js
setTimeout(() => {
  console.log("Asynchronous JavaScript");
}, 2000);

console.log("Hello World");
console.log("Goodbye World");

// Output:
// Hello World
// Goodbye World
// Asynchronous JavaScript
```
