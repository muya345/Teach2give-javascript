# Type Coercion and Type Conversion
Type coercion and type conversion involve changing a value from one data type to another, but they differ in how they happen.
## Type Coercion (Implicit Conversion)
Happens automatically when JavaScript tries to perform operations between different data types.

Common in comparisons (`==`), string concatenation (`+`), and arithmetic operations.

Type coercion sometimes leads to unexpected results.

Examples:
```javascript
console.log(6 + "6"); // "66" (Number coerced into a string)
console.log("6" - 3
); // 3 (String coerced into a number)
console.log(true + 2
); // 3 (true coerced into 2)
console.log(false + "10"); // "false10" (false coerced into string)
```
## Type Conversion (Explicit Conversion)
Happens when you manually convert the data type of a value.

### Methods of Explicit Conversion
- Convert to string using `String()` or `toString()`.
```javascript
console.log(String(283));
console.log((283).toString());
```
- Convert to number using `Number()`, `parseInt()` or `parseFloat()`
```javascript
console.log(Number("283"));
console.log(parseInt("283"));
console.log(parseFloat("283"));
console.log(parseInt("32px"));
```
- Convert to boolean using Boolean()

- Falsy values: `0`, `""`, `null`, `undefined`, `NaN`, `false`.

- Truthy values: everything else
```javascript
console.log(Boolean(0)); // false
console.log(Boolean("hello")); // true
console.log(Boolean(null)); // false