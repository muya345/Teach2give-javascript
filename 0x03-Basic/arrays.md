# Arrays
It is a collection of elements of the same type stored in contiguous memory locations.
it can hold multiple values in a single variable.
it can be referenced using index.

## Creating an array
You can create using the following ways:
- An array literal
- The new `Array()`constructor.
### Using an array literal
```js
const arrayName = ["value1", "value2", "value3"];
Example:
const colors = ["red", "green", "blue"];
```
You can also nest arrays within arrays (multidimensional arrays):
```js
const arr = [[1, 2, 3], [4, 5, 6], [7, 8, 9]];
```

### Using the `new Array()` constructor
```js
const arrayName = new Array(value1, value2, value3);
```
Example:
```js
const colors = new Array("red", "green", "blue");
```
`new Array() ` constructor can also be nested:
```js
const arr = new Array(new Array(1, 2, 3), new Array(4, 5, 6), new Array(7, 8, 9));
``` 
## Accessing an array
You  can access an array using index.
The first element has index 0, the second element index 1, e.t.c.
```js
const colors = ["red", "green", "blue"];
console.log(colors[0]); // Output: "red"
console.log(colors[1]); // Output: "green"
console.log(colors[2]); // Output: "blue"
```
## Basic Array methods
### length of an array
The `length` property returns the sizeof elements in an array.
```js
const colors = ["red", "green", "blue"];
console.log(colors.length); // Output: 3
```
### `pop()`
The `pop()` method removes the last element from an array and returns that element.
```js
const colors = ["red", "green", "blue"];
console.pop()
console.log(colors); // Output: ["red", "green"]

```
`push()`
The `push()` method adds one or more elements to the end of an array and returns the new length of the array.
```js
const colors = ["red", "green", "blue"];
colors.push("yellow");
console.log(colors); // Output: ["red", "green", "blue", "yellow"]
```
You can also add multiple elements using the `push` method:
```js
const colors = ["red", "green", "blue"];
colors.push("yellow", "orange");
```
The push method returns the new length of the array.

### `shift()`
It removes the first element from an array and returns that element.
```js
const colors = ["red", "green", "blue"];
colors.shift();
console.log(colors); // Output: ["green", "blue"]
```

### `unshift()`
it adds an element to the start of an array.
```js
const colors = ["red", "green", "blue"];
colors.unshift("yellow");
console.log(colors); // Output: ["yellow", "red", "green", "blue"]
```
You can also add multiple elements using the `unshift` method:
```js
const colors = ["red", "green", "blue"];
colors.unshift("yellow", "orange");
```
 ### `at()`
The `at()` method returns the element at the specified index in an array.
```js
const colors = ["red", "green", "blue"];
console.log(colors.at(1)); // Output: "green"
console.log(colors.at(-1)); // Output: "blue"
```
### `join()`
it joins all array elements into a string.
It behaves just like toString(), but in addition, you can specify the separator:
```js
const colors = ["red", "green", "blue"];
console.log(colors.join("-")); // Output: "red-green-blue"
```
### `concat()`
It creates a new array by merging two or more arrays.
```js
const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];
console.log(arr1.const(arr2));
//{'1' '2' '3' '4' '5' '6' }
```
### `flat()`
It converts a multidimensional array to a one dimension array.
```js
const colour = [
  ["red", "green"],
  ["black", "red"],
  ["yellow", "pink"],
];
console.log(colour.flat());
// ['red', 'green', 'black', 'red', 'yellow', 'pink']
```
### `indexOf()`
It is used to fix the index of an element.
It returns -1 if the element is not found.
```js
const colour= ["red", "green", "pink", "blue"];
console.log(colour.indexOf("pink")); // 3
```
### `reverse()`
Reverses the elements of an array.
```js
const colour = ["red", "blue", "pink", "green"];
console.log(colour.reverse());





