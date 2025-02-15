# Variables
In javascript, a a variable is a labeled container that holds a piece of information
# Declaring Variables in JavaScript
1. `var`: old, not recommended for modern code

2. `let`: preferred for variables that change

3. `const`: used for values that should not change
```javascript
let age = 23// A variable named "age" holding the value 25
const name = "Stella"constant variable holding a text value
var city = "Nairobi" of declaring variables
```
## Updating Variables
We use `let` and `val`
```javascript
let score = 13
score = 17 // Now the value of "score" is updated to 17

var player = ""GK"
player = "Martinez"
```
But `const` cannot be changed once assigned
```javascript
const country = "Kenya";
country = "Uganda"; // ❌ This will cause an error!
```
# Declaring vs. Initializing variables
# Declaring Variables
eclaring a variable means creating it without assigning a value. This tells JavaScript that a variable exists, but it does not have any value yet.
When you try to read the value of a variable that has been declared but has not been initialized, you will get undefined as the outpu
```javascript
let age; // Declared but not initialized
console.log(age); // Output: undefined
```
You can then define the variable later
```javascript
let age; // Declared but not initialized
age = 23
console.log(age); // Output: 23
```
# Initializing a variable
it means assigning it an initial value at the time of declaration.
```javascript
let age = 23 // Declared AND initialized with a value
console.log(age); // Output: 23
```
NOTE: `const` must be initialized immediately
# Rules for naming variables
Variable names can only start with a letter, underscore (_), or dollar sign ($)
✅Valid examples:
```javascript
let name = "Stella"
let _score ="80"
let $price = 44.00
```
❌ Invalid Example:
```javascript
let 1stPlace = "Gold"; // ❌ Cannot start with a number
```
### Variable names cannot be JavaScript reserved keywords
❌ Invalid Examples:
```javascript
let let = "Hello"; // ❌ "let" is a reserved keyword
let function = 24 // ❌ "function" is a reserved keyword
```
Variable names can only contain letters, numbers, underscore and the dollar sign, no special characters or spaces
✅ Valid Examples:
```javascript
let userAge = 23
let _totalAmount = 80
let $discount = 4
```
❌ Invalid Example:
```javascript
let user-age =-24 ❌ Hyphens are not allowed
let total amount = 80 // ❌ Spaces are not allowed
```
### Variable names are case-sensitive
Variable names are case-sensitive
```javascript
let Age = 35
let age = 30
console.log(Age); // 35
console.log(age); // 30
```
Even though the names look similar, they are treated as separate variables.
### Use meaningful and descriptive names
✅ Good Practice:
```javascript
let userName = "jeff"
let totalPrice = 100
let isLoggedIn = true;
```
❌ Bad Practice:
```javascript
let x = "Jeff/ ❌ Not descriptive
let tp = 100 // ❌ Unclear what "tp" stands for
```
If a variable name is made up of multiple words, use the camel case convention
```javascript
let userName = "Jeff"
let totalPrice = 100
let isLoggedIn = true;
```




