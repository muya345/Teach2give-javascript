# Javascript classes
A class refers to the blueprint of an object.

## Creating a class﻿
To create a class in JavaScript, you use the class keyword followed by the class name. Inside the class, you define a constructor method to initialize object properties.
```js
class User {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  greet() {
    console.log(`My name is ${this.name}`);
  }
}
```
## Creating instances of a class
To create an instance of a class, use the `new` keyword.
```js
class User {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  greet() {
    console.log(`My name is ${this.name}`);
  }
}

const user1 = new User("Jeff Benzos", 59);
user1.greet(); // My name is Jeff Benzos
```
