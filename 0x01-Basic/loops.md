# Loops
They enable us to repeat a block of code multiple times.
They include:
- while loop
- for loop
- do-while loop

## while loop
Runs ass long as specified condition is true.
```javascript
while (condition) {
  // code block to be executed if condition is true
}
```
```javascript
let num = 2;

while (num <= 5) {
  console.log("Number ", num);
  num++;
}
```

## for loop
Used to execute a block of code a specified number of times.
The syntax is:
```javascript
for (initialization; condition; update) {
    // code
}
```
- initialization: Used to initialize a variable used in the loop.
- Condition is used to evaluate the condition of the initial variable, if the condition returns true, the loop starts over again, if the condition returns false, the loop ends.
- Update is used to update the initialized variable.

```javascript
for (let i = 1; i <= 5; i++) {
    console.log("Iteration:", i);
}
```

## do-while loop
Executes the loop at least once, even if the condition is `false` from the start.

```javascript
do {
  /* code of block that will be
     executed at least once even if
     condition is false */
} while (condition);
```

```javascript
let y = 2;

do {
  console.log("y ", y);
  x++;
} while (y <= 5);
```
## break and continue statements
`break` and `continue` statements are keywords that are always used within a loop.

### `break` statement
it is used when we want to terminate the running loop whenever any particular condition occurs.
Whenever a `break` statement occurs, the loop breaks and stops executing.
The `break` statement exits the loop completely.

```javascript
for (let x = 1; x < 10; x++) {
  if (x == 5) {
    break;
  }
  console.log(x);
}
```

### continue statement
It is used to skip the current iteration of the loop and `continue` to the next iteration.
Whenever we write `continue` statement, the whole code after that statement is skipped and the loop will go for the next iteration.

The `continue` statement skips the current iteration and moves on to the next iteration.

```javascript
for (let x = 1; x < 10; x++) {
  if (x == 5) {
    continue;
  }
  console.log(x);
  }
```





