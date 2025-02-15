# Data Types
Basic datatypes:
-String 
-Number
-Boolean
-null
-undefined
-Bigint
-Symbol
## String
Refers to a sequence of characters enclosed within single quotes ('), double quotes (") or backticks
```javascript
let firstName = "jeff"
let lastName = "cess"
let username = `jeff cess"
```
## Numbers
JavaScript has only one type for numbers: it can store both integers and decimals
```javascript
let age = 23 // Integer
let price = 92.99 // Decimal
let notANumber = NaN; // Not a Number (invalid math operation)
```
## Boolean
Boolean can either be `true` or `false`.
```javascript
let isMale = true;
let isFemale = false;
```
## underfined

Refers to a variable that has been declared but not initialized
```javascript
let country;
console.log(country); // Output: undefined
```
## null
`null` is an intentional absence of a value. Unlike `undefined`, which means "not assigned," null means "empty on purpose."
```javascript
let car = null; // No car yet
```
## Bigint
Used for numbers beyond JavaScript’s Number.MAX_SAFE_INTEGER (9,007,199,254,740,991)
```javascript
let bigNumber = 09887654321098765432109876n; a BigInt
console.log(bigNumber);
```
# Checking the type of a variable using the `typeof` operator
We use the `typeof` 
```javascript
let bigNumber = 09876543210987654321109866n;
console.log(typeof bigNumber); // bigint
// OR
console.log(typeof bigNumber); // bigint

const age = 23
const fullName = "Jeff"

console.log(typeof age); // number
console.log(typeof fullName); // string

