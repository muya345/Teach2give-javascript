# Operators
They are symbols that perform opeations on values (operands).
Used for calculation, comparison, and logical operations.
Operators are classified into the following categories
-Arithmetic operators: perform basic mathematical operations.

- Assignment operators: assign values to variables.

- Comparison operators: compare values.

- Logical operators: used for boolean logic.

- Bitwise operators: perform operations at the binary level.

- Ternary operators

- Type operators
## Arithmetic Operators
Used to perform mathematical operations.
## =(addition)
Add two numbers:
```javascript
let a = 20
let b = 5;
console.log(a + b); //25
```
It can also be used with strings to perform string concatenation
```javascript
let firstName = "Jeff"
let lastName = "cess"
console.log(firstName + lastName); // Jeffcess
```
## -(subtraction)
Subtract the right operand from the left:
```javascript
let a = 20
let b = 5;
console.log(a - b); // 15
```
## *(multiplication)
Calculates the product of two numbers:
```javascript
let a = 20
let b = 5;
console.log(a * b); // 100
```
## / (Division)
```javascript
let a =20
let b = 5;
console.log(a / b); //4
```
## % (modulus/remainder)
Returns the remainder of the division between the left and right operand
```javascript
let a = 20
let b = 5;
console.log(a % b); // 0
```
## ** (Exponentiation)
```javascript
let a = 20
let b = 5;
console.log(a ** b); // 200000
```
## Increment Operator
Increases the variable's value by 1.

It can be used in two ways:
- Post-increment (`a++`): returns the original value and then increments it

- Pre-increment (`--a`): increments first then returns the updated value
```javascript
let x = 6;
console.log(x++); // 6 (returns first, then increments)
console.log(x); // 7

let y = 6;
console.log(++y); // 7 (increments first, then returns)
```
## Decrement Operator
Decreases the variable's value by 1.

It can be used in two ways:

- Post-decrement (`a--`): returns the original value, then decrements.

- Pre-decrement (`--a`) – decrements first, then returns the updated value
# Assignment Operators
Used to assign values to variables

## = (Simple assignment operator)
Used to assign a value to a variable
```javascript
let x = 10;
```
## += (Addition assignment operator)
Used to add a value to a variable
```javascript
let x = 10;
x += 5; // x = x + 5 → 15
```
## -= (Subtraction assignment operator)
Subtracts a value from a variable
```javascript
let x = 5;
x -= 2; // x = x - 2 → 3
```
## *= (Multiplication assignment operator)
Multiples a variable
```javascript
let x = 5;
x *= 2; // x = x * 2 → 10
```
## /= (Division Assignment Operator)
Divides a variable
```javascript
let x = 15;
x /= 3; // x = x / 3 → 5
```
# Comparison Operators
They are used to compare values and they return `true` or `false`.

## == (Equality Operator)
Returns true if the operand on the left is equal to the operand on the right and false otherwise
```javascript
let a = 10;
let b = 5;
console.log(a == b); // false
console.log(a == 10); // true
```
Note: The equality operator ignores the data type of the operands, it only compares the value:
```javascript
console.log(10 == "10"); // true
```
## === (Strict equality operator)
Returns true if the operand on the left is equal to the operand on the right and false otherwise.
```javascript
let a = 10;
let b = 5;
console.log(a === b); // false
console.log(a === 10); // true
```
Note: The strict equality operator checks the data type as well, not just the values:
```javascript
console.log(10 === "10"); // false
```
## != (Not equal/Inequality operator)
Returns true if the value on the left is not equal to the value on the right and false otherwise.

It does not consider the data type of the operands.
```javascript
let a = 10;
let b = 5;
console.log(a != b); // true
console.log(a != 10); // false

console.log(10 != "10"); // false
```
## !== (Strict not equal to/Strict inequality operator)
Returns true if the value on the left is not equal to the value on the right and false otherwise.

It compares the data types of the operands.
```javascript
let a = 15;
let b = 10;
console.log(a !== b); // true
console.log(a !==15); // false

console.log(15 !== "15"); // true
```
>## (Greater than)
Returns true if the operand on the left is greater than the operand on the right and false otherwise.
```javascript
let a = 15;
let b = 10;
console.log(a > b); // true
console.log(b > a); // false
```
## < (Less than)
Returns true if the operand on the left is less than the operand on the right and false otherwise.
```javascript
let a = 15;
let b = 10;
console.log(a < b); // false
console.log(b < a); // true
```
## >= (Greater than or equal to)
Returns true if the operand on the left is greater than or equal to the operand on the right.
```javascript
let a = 15;
let b = 10;
console.log(a >= b); // true
console.log(b >= a); // false
console.log(15 >= 15); // true
```
## <= (Less than or equal to)
Returns true if the operand on the left is less than or equal to the operand on the right.
```javascript
let a = 15;
let b = 10;
console.log(a <= b); // false
console.log(b <= a); // true
console.log(15 <= 15); // true
```
# Logical Operators
Used for boolean logic.

Logical AND Operator (&&)
The AND operator returns true only if both operands are true; otherwise, it returns false.
```javascript
console.log(true && true); // true
console.log(true && false); // false
```
Truth table for the AND operator.






## Logical OR Operator (||)
The OR operator returns true if at least one of the operands is true; otherwise it returns false.
```javascript
console.log(true || true); // true
console.log(true || false); // true
console.log(false || false); // false
```
## Logical NOT operator (!)
Used to negate boolean value of an expression, it returns true if the expression is false and returns false if the expression is true.
```javascript
console.log(!true); // false
console.log(!false); // true
```




