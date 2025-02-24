# Arrow functions
Arrow functions `(=>)` provide a more concise syntax for writing functions in JavaScript.

They remove the need for the function keyword and have a shorter syntax.
```js
Before
function add(1, 2
) {
  return 1 + 2;
}
 
console.log(add(4, 12));
After
const add = (1, 2) => 1 + 2;
 
console.log(add(4, 12));
```
Arrow functions don't have their own `this` keyword. This means they cannot be used as object methods.
