# Sets
It is a collection of unique values.

## Properties of a set﻿
- Unique elements: sets cannot contain duplicate elements.

- No indexing: elements in a set are not accessed by their position.

- No order: unlike arrays, elements in a set don't maintain their order.

## Creating a set
use `new Set()`
```javascript
const myset = new Set([1, 2, "a", "Jeff"]);
console.log(myset);
```
## Set Methods
### `add(value)`
 Adds a value to a specific  set.
```javascript
const myset = new Set();
myset.add(1);
myset.add(2);
myset.add("a");
myset.add("Jeff");
myset.add("Benzos");
myset.add(true);
myset.add(true);
myset.add(false);
console.log(myset); // Set(6) { 1, 2, "a", "Jeff", "Benzos", true false }
```
### `delete(value)`
Removes a value from a specific set.
```javascript
const myset = new Set([1, 2, "a", "Jeff"]);
myset.delete(1);
myset.delete(2);
console.log(myset); // Set(2) { "a", "Jeff" }
``` 
### `has(value)`
Returns `true` if the value exists in the set, otherwise returns `false`.
```javascript
const myset = new Set([1, 2, "a", "Jeff"]);
console.log(myset.has(1)); // true
console.log(myset.has(0)); // false
```
### `size`
Returns the number of elements in the set.
```javascript
const myset = new Set([1, 2, "a", "Jeff"]);
console.log(myset.size); // 4