# Functions
Functions are blocks of code that are executed when they are called.
Functions can be used to break down a complex task into smaller, more manageable parts.
Functions can also be used to reuse code.
Functions are defined using the `function` keyword followed by a name, followed by parentheses.
```javascript
function functionName() {
  // function body
}
```
```javascript
function printHello() {
  console.log("Hello, world");
}
```
To use a function, you must call/invoke the function as shown:
```javascript
function printHello() {
  console.log("Hello, world");
}

// calling/invoking a function
printHello();
```
## Parameters vs Arguments
A parameter is a variable declared in a function definition and acts as a placeholder for the value that will be passed to the function when the function is being called.

An argument is the actual value passed to a function when it is called, it provides the data that the function or the method will operate on

```javascript
function greet(name) { // name is a parameter
  console.log(`Hello ${name}`);
}

greet("Jeff Cess"); // Jeff Cess is an argument
```
## Function return values
A function can return a value using the `return` keyword.
```javascript
function add(num1, num2) {
  return num1 + num2;
}

let result = add(2, 3);
console.log(result); // 5
```
## Categories of functions
- Functions that don't take parameter(s) and don't return a value

- Functions that don't take parameter(s) but return a value

- Functions that take parameter(s) but don't return a value.

- Functions that take parameter(s) and return a value.

### Functions that don't take parameter(s) and don't return a value
These functions don't take any parameter(s) and don't return any values.

```javascript
function add() {
  let x = 40;
  let y = 55;
  console.log(x + y);
}

add();
```
### Functions that  take parameter(s) but don't return a value
```javascript
function add(x, y) {
  console.log(x + y);
}
add(4, 5);
```
### Functins that take parameter(s) and return a value
```javascript
function add(x, y) {
  return x + y;
}

let result = add(4, 5);
console.log(result); // 9
```
## Types of functions in JavaScript
- Function declaration

- Function expression/anonymous function

- Arrow functions

- Immediately Invoked Function Expression (IIFE)

- Callback functions

### Function declaration
```javascript
function add(x, y) {
  console.log(x + y);
}

add(5, 2);
```
### Function expression/anonymous function
```javascript
let add = function(x, y) {
  console.log(x + y);
}

add(5, 2);
```
### Arrow functions
```javascript
let add = (x, y) => {
  return x + y;
}

console.log(add(5, 2));
```
If an arrow function has only one line in the body, we can get rid of the curly braces.

This means that instead of:




```javascript
let add = (x, y) => {
    console.log(x + y);
}

add(5, 2);
```

can be written as:

```javascript
let add = (x, y) => console.log(x + y);
```


If an arrow function has only one line of code in the body and that line happens to be a return statement, we can get rid of the return keyword:

```javascript
let add = (x, y) => x + y;
console.log(add(5, 2));
```
If an arrow function has only one parameter, we can get rid of the parenthesis:

```javascript
let square = number => number * number;

console.log(square(8)); // 64
```

### Immediately Invoked Function Expression (IIFE)
```javascript
(function() {
  console.log("Hello, world");
})
();
```
These functions can also take parameters:

```javascript
(function (x, y) {
    let sum = x + y;
    let product = x * y;
    console.log(`Sum: ${sum}, Product: ${product}`);
    console.log(`Sum: ${sum}, Product: ${product}`);
})(2, 3);
```

### Callback functions
 Refer to functions passed as arguments to other functions.

```javascript
functional greet(name, callback) {
  console.log(`Hello ${name}`);
  callback();
}
greet("Jeff Cess", function() {
  console.log("This is a callback function");
})  
```

    

