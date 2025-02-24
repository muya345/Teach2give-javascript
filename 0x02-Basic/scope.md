# Scope
Scope in JavaScript determines where variables are accessible.

It determines the accessibility (visibility) of variables.

JavaScript has the following types of scope:

- Global Scope

- Function Scope (local scope)

- Block Scope (introduced in ES6)

- Lexical scope

## Global Scope
Variables declared outside of any function or block are called global variables.

```javascript
let x = 10;
function exampleFunction() {
    console.log(x); // accessible inside the function
}

exampleFunction(); 10
console.log(x); // accessible outside the function
```
## Function Scope
Variables declared inside a function are accessible only within that function.

They cannot be accessed outside the function.

```javascript
function exampleFunction() {
    let x = 10;
    console.log(x); // works inside the function
}
console.log(x); // ReferenceError: x is not defined
```

## Block Scope (`let` and `const`)
A block is any code inside curly brackets `{}` (e.g., in `if`, `for`, `while` statements).

```javascript
if (true) {
    let x = 10;
    console.log(x); // works inside the block
}
console.log(x); // ReferenceError: x is not defined
```
Variables declared with `let` and `const` are only accessible inside the block they are declared in.

`var` does not follow block scope.

## Lexical Scope
It means that a function can access variables from its parent scope (e.g., parent function).

```javascript
function parentFunction() {
    let x = 10;
    function innerFunction() {
        console.log(x); // 10
    }
    innerFunction();
}
parentFunction();

