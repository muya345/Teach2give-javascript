# Objects
An object is a collection of key-value pairs.
It is a data structure that stores values as a collection of key value pairs.

The key must always be a string, and the value can be of any type.

Keys are also referred to as properties.

Objects are one of the most fundamental data structures in JavaScript.

A function inside an object is called a method.
## Creating Objects
- Object literal
- Object constructor function
- Using `new Object()`
### Object literal
The simplest way to create an object is to use curly braces, this is referred to as object literal.

```javascript
let person = {
    firstname: "Jeff",
    lastname: "Bezos",
    age: 59,
    isAlive: true,
    greet: function() {
        console.log("Hello, World");
    }
};
```
### Using new `Object()`
`new Object()` creates an empty object. It's functionally equivalent to object literal but rarely used in modern JavaScript.
```javascript
let person = new Object();
person.firstname = "Jeff";
person.lastname = "Bezos";
person.age = 59;
person.isAlive = true;
person.greet = function() {
    console.log("Hello, World");
};
```
### Using a Constructor Function
It is a regular function used with the `new` keyword to create a new object with shared properties and method.
```javascript
function Person(firstname, lastname, age, isAlive) {
    this.firstname = firstname;
    this.lastname = lastname;
    this.age = age;
    this.isAlive = isAlive;
    this.greet = function() {
        console.log("Hello, World");
    };
}
const person = new Person("Jeff", "Bezos", 59, true);
```
## Accessing Object Properties
There are two ways:
- Dot notation
- Bracket notation
### Dot notation
it allows you to access a property of an object using a period followed by the property name.
```javascript
let person = {
    firstname: "Jeff",
    lastname: "Bezos",
    age: 59,
    isAlive: true,
    greet: function() {
        console.log("Hello, World");
    }
};
console.log(person.firstname); // "Jeff"
console.log(person.lastname); // "Bezos"
```
### Bracket notation
It accesses an object's properties using square brackets `([])` with the property name as a string.
```javascript
let person = {
    firstname: "Jeff",
    lastname: "Bezos",
    age: 59,
    isAlive: true,
    greet: function() {
        console.log("Hello, World");
    }
}
console.log(person["firstname"]); // "Jeff"
console.log(person["lastname"]); // "Bezos"
console.log(person["age"]); // 59
console.log(person["isAlive"]); // true
```
### Modifying Object
#### Adding new properties
You can use the dot or bracket notation to add new properties to an object.
```javascript
let person = {
    firstname: "Jeff",  
    lastname: "Bezos",
    age: 59,
    isAlive: true,
    greet: function() {
        console.log("Hello, World");
    }
};
person.job = "CEO";
person["company"] = "Amazon";
```
### Updte existing properties
```javascript
let person = {
    firstname: "Jeff",  
    lastname: "Bezos",
    age: 59,
    isAlive: true,
    greet: function() {
        console.log("Hello, World");
    }
}
person.age = 60;
person.isAlive = false;
```
### Deleting properties
```javascript
let person = {
    firstname: "Jeff",  
    lastname: "Bezos",
    age: 59,
    isAlive: true,
    greet: function() {
        console.log("Hello, World");
    }
};
delete person.age;
delete person.isAlive;
```
## Checking properties in an object
You can use:
- `in` operator
- `hasOwnProperty()` method

### `in` operator
```javascript
let person = {
    firstname: "Jeff",  
    lastname: "Bezos",
    age: 59,
    isAlive: true,
    greet: function() {
        console.log("Hello, World");
    },
};
console.log("age" in person); // true
console.log("job" in person); // false
```
### `hasOwnProperty()` method
```javascript
let person = {
    firstname: "Jeff",  
    lastname: "Bezos",
    age: 59,
    isAlive: true,
    greet: function() {
        console.log("Hello, World");
    },
};
console.log(person.hasOwnProperty("age")); // true
console.log(person.hasOwnProperty("job")); // false
```
##  Object Methods
### `Object.keys(objectName)`
Returns an array containing all the keys of an object.
```javascript
let person = {
    firstname: "Jeff",  
    lastname: "Bezos",
    age: 59,
    isAlive: true,
    greet: function() {
        console.log("Hello, World");
    },
};
console.log(Object.keys(person)); // ["firstname", "lastname", "age", "isAlive", "greet"]
```
### `Object.values(objectName)`
Returns an array containing all the values of an object.
```javascript
let person = {
    firstname: "Jeff",  
    lastname: "Bezos",
    age: 59,
    isAlive: true,
    greet: function() {
        console.log("Hello, World");
    },
};
console.log(Object.values(person)); // ["Jeff", "Bezos", 59, true, [Function: greet]]
```
### `Object.entries(objectName)`
Returns an array containing all the key-value pairs of an object.
```javascript
let person = {
    firstname: "Jeff",  
    lastname: "Bezos",
    age: 59,
    isAlive: true,
    greet: function() {
        console.log("Hello, World");
    },
};
console.log(Object.entries(person)); // [["firstname", "Jeff"], ["lastname", "Bezos"], ["age", 59], ["isAlive", true], ["greet", [Function: greet]]]
```
### `Object.freeze(objectName)`
Freezes an object, preventing changes to the object.
```javascript
let person = {
    firstname: "Jeff",  
    lastname: "Bezos",
    age: 59,
    isAlive: true,
    greet: function() {
        console.log("Hello, World");
    },
};
Object.freeze(person);
person.middleName = "Cess" // won't work
```
## Iterating over an object using the `for..in` loop
You can use `for..in` loop to iterate over an object as shown:
```javascript
let person = {
    firstname: "Jeff",
    lastname: "Benzos",
    age: 59,
    isAlive: true,  
    greet: function() {
        console.log("Hello, World");
    },
};
for (let key in person) {
    console.log(key)
}
```
The for..in loop can also be used to loop over arrays.





    

