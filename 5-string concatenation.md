# String Concatenation
It is the process of two or more strings together
JavaScript provides multiple ways to concatenate strings.
# 1. Using the + Operator
```javascript
let firstName = "Jeff";
let lastName = "Cess";
let fullName = firstName + lastName;
console.log("My full name is " + fullName);
```
# 2. Using the += operator to append to an existing string
```javascript
let message = "Hello ";
message += "Stella.";
console.log(message);
```

# Using Template Literals
Template literals (introduced in ES6) use backticks (`) and '${}' placeholders for variables.
```javascript
let firstName = "Jeff";
let lastName = "Cess";
console.log(`My name is ${firstName} ${lastName}`);
```


