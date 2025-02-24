# High Order Array Methods
They include:
## `forEach`
Executes a function once for each array element but does not return anaything

```js
const numbers = [1, 2, 3, 4, 5];

numbers.forEach((number) => {
    console.log(number * 2);
});
// 2, 4, 6, 8, 10
```
## `map`
Creates a new array populated with the results of calling a provided function on every element in the calling array

```js
const numbers = [1, 2, 3, 4, 5];

const newNumbers = numbers.map((number) => {
    return number * 2;
});
// [2, 4, 6, 8, 10]
```
## `filter`
Creates a new array with all elements that pass the test implemented by the provided function
```js
const numbers = [1, 2, 3, 4, 5];

const newNumbers = numbers.filter((number) => {
    return number % 2 === 0;
});
// [2, 4]
```
## `reduce`
Executes a reducer function on each element of the array resulting in a single value
```js
const numbers = [1, 2, 3, 4, 5];

const total = numbers.reduce((total, number) => {
    return total + number;
}, 0);
// 15
```
## `find`
Returns the value of the first element in the array that satisfies the provided testing function
```js
const numbers = [1, 2, 3, 4, 5];

const number = numbers.find((number) => {
    return number % 2 === 0;
});
// 2
```
## `findIndex`
Returns the index of the first element in the array that satisfies the provided testing function
```js
const numbers = [1, 2, 3, 4, 5];

const index = numbers.findIndex((number) => {
    return number % 2 === 0;
});
// 1
```
Checks if at least one element passes a condition.
If so, it returns true, otherwise, it returns false.
```js
const numbers = [1, 2, 3, 4, 5];

const result = numbers.some((number) => {
    return number % 2 === 0;
});
// true
```
## `every`
Checks if all elements pass a condition.
If so, it returns true, otherwise, it returns false.
```js
const numbers = [1, 2, 3, 4, 5];

const result = numbers.every((number) => {
    return number % 2 === 0;
});
// false
```

