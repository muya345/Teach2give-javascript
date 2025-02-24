# Conditionals 
it allows you to execute different blocks of code based on specific conditions.
They include:
- if statement
- if else statement
- if else ladder
- switch statement

## if statement
Used to execute a block of code if a specified condition is true.
ie:
```javascript
if (condition) {
  // block of code to be executed if the condition is true
}
```
Example in code:
```javascript
let position = 3;
if (position < 5) {
  console.log("You are qualified");
}
```

## if else statement
Executes the code in the `if` block when the condition is true, if the condition is false, the code inside the else block gets executed.
```javascript
if (condition) {
  // block of code to be executed if the condition is true
} else {
  // block of code to be executed if the condition is false
}
```
Example in code:
```javascript
let position = 3;
if (position < 5) {
  console.log("You are quarified");
} else {
  console.log("You are dismissed");
}
```
## if else ladder
Used when multiple conditions need to be checked sequentially.

The syntax is as follows:
```javascript
if (condition1) {
  // block of code to be executed if condition1 is true
} else if (condition2) {
  // block of code to be executed if condition1 is false and condition2 is true
} else {
  // block of code to be executed if both condition1 and condition2 are false
}
```
Example in code:
```javascript
let age = 74;
if (age >= 60) {
  console.log("Eldery");
} else if (age >= 40 && marks < 60) {
  console.log("Aldult");
} else if (age >= 18 && marks < 40) {
  console.log("Youth");
} else {
  console.log("Child");
}
```
## Switch Statemants
Used when a variable has multiple possible values. It’s cleaner than multiple `if..else` if conditions.
ie:
```javascript
switch (expression) {
  case value1:
    // block of code to be executed if expression === value1
    break;
  case value2:
    // block of code to be executed if expression === value2
    break;
  default:
  // block of code to be executed if expression doesn't match any case
}
```
Example in code:
```javascript
let month= "January";
switch (month) {
  case "January":
    console.log("Start of the year month.");
    break;
  case "December":
    console.log("End of year is near!");
    break;
  case "December":
    console.log("It's a holiday.");
    break;
  default:
    console.log("It's a regular month.");
}
```
## Ternary Operator
It provides a concise way to write a simple if-else statement.

The syntax is as follows:
```javascript
condition ? expression if condition is true : expression if condition is false
```
Example in code:
```javascript
const position = 3;

age < 5 ? console.log("You are qualified") : console.log("You are dismissed");
```


