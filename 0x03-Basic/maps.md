# Maps
A map data structure is similar to an object, in that it allows you to store key-value pairs.

## Creating a map
using `new Map()`
```javascript
const mymap = new Map();
```
## Maps method
Adds a key-value pair to a specific map.
```javascript
const mymap = new Map();
mymap.set("name", "Jeff");
mymap.set(1, number);
mymap.set([1, 2, 3], "array");
mymap.set([true, "boolean value"], "array");
mymap.set( { username: "the_user" }, "object");
console.log(mymap);
    // Map(5) {
    //     "name" => "Jeff",
    //     1 => number,
    //     [ 1, 2, 3 ] => "array",
    //     [ true => 'boolean value' ] => "array",
//     { username: 'the_user' } => "object"
// }
```
### `get(key)`
Returs value associated with a specific key.
```javascript
const mymap = new Map();
mymap.set("name", "Jeff");
mymap.set(1, number);
mymap.set([1, 2, 3], "array");
mymap.set([true, "boolean value"], "array");
mymap.set({username: "the_user"}, "object");

console.log(mymap.get(1)); // number
console.log(myMap.get("firstName")); // Jeff
console.log(myMap.get("something")); // undefined
```
### `has(key)`
Returns true if the map contains the specified key, false otherwise
```JavaScript
const myMap = new Map();
myMap.set("firstName", "Jeff");
myMap.set(1, "number");
myMap.set([1, 2, 3], "array");
myMap.set(true, "boolean value");
myMap.set({ username: "the_user" }, "object");

console.log(myMap.has("firstName")); // true
console.log(myMap.has("middlename")); // false
```
### `delete(key)`
Removes a specified key-value pair from the map.
```JavaScript
const myMap = new Map();
myMap.set("firstName", "Jeff");
myMap.set(1, "number");
myMap.set([1, 2, 3], "array");
myMap.set(true, "boolean value");
myMap.set({ username: "the_user" }, "object");

myMap.delete("firstName");
myMap.delete(1);
```
### `clear()`
Removes all the key-value pairs from a map.

```JavaScript
const myMap = new Map();
myMap.set("firstName", "Jeff");
myMap.set(1, "number");
myMap.set([1, 2, 3], "array");
myMap.set(true, "boolean value");
myMap.set({ username: "the_user" }, "object");

myMap.clear();

console.log(myMap); // Map(0) {}
```
### `size`
Returns the number of key-value pairs in a map.
```JavaScript
const myMap = new Map();
myMap.set("firstName", "Jeff");
myMap.set(1, "number");
myMap.set([1, 2, 3], "array");
myMap.set(true, "boolean value");
myMap.set({ username: "the_user" }, "object");

console.log(myMap.size); // 5












