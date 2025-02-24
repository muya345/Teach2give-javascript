# Template literals
Also known as template strings
They allow:

- Multi-line strings without `\n`.

- String interpolation (injecting variables to strings).

- Embedded expressions.

- e.t.c.

Template literals use backticks instead of single or double quotes.

## String interpolation: Injecting variables into strings
Before ES6, inserting variables into a string required concatenation (+), which was cumbersome.

With template literals, introduced in ES6, this has been made easier:

Before template literals:
```js
const username = "Jeff";
const age = 59;

console.log("My name is " + username + " and I am " + age + " years old.");
// My name is Jeff and I am 59 years old.
```

With template literals:
```js
const username = "Jeff";
const age = 59;
console.log(`My name is ${username} and I am ${age} years old.`);
```
## Multi-line strings(without `\n`)
Before ES6, multi-line strings required `\n` or joining with `+`:
```js
const multiline = "This is a \n + "Tis is line b/n" + "This is line c/n";
console.log(multiline);
/*
This is line a
Tis is line b
This is line c
*/
```
```js
const multiline = `This is line a
Tis is line b
This is line c`;
console.log(multiline);
/*
This is line a
Tis is line b
This is line c
*/
```
## Expressions inside template literals
Template literals can evaluate expressions directly inside `${}`
```js
let a = 1;
let b = 2;

function add(a, b) {
    return a + b;
}

console.log(`The sum of ${a} and ${b} is ${add(a, b)}.`);
```
