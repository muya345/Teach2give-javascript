# Promises
When working with asynchronous JavaScript, there is the concept of producing code and consuming code.

- Producing code: is code that will take some time to complete e.g. fetching user information from a database.

- Consuming code: code that must wait for results from producing code

- A promise is an object that links producing and consuming code.

- It is an object that also represents the eventual completion (or

A promise has three states:

- Pending: initial state; neither fulfilled nor rejected.

- Fulfilled: the operation is completed successfully.

- Rejection: the operation has failed.

## Creating a promise
A promise is created using the new `Promise()` constructor.

The `new Promise()` constructor accepts a single argument, which is a function called executor.

The promise executes the executor function immediately.
```js
let promise = new Promise((resolve, reject) => {
    let a = 2;
    if (a === 2) {
        resolve(!"a is 2";
    } else {
        reject("a is not 2");
    }
    });
```
# Consuming a promise
We can then use `.then()` to handle resolved value and `.catch()` to handle errors (rejected value).

`.then()` takes a callback function, which receives the resolved value of the Promise as its argument.

`.catch()` also takes a callback function, which receives the error (rejected value) as its argument when the Promise is rejected.
```js
let myPromise = new Promise(function (resolve, reject) {
  let x = 5;
  if (x === 1) {
    resolve("x is 1");
  } else {
    reject("x is not 1");
  }
});

myPromise
  .then((result) => {
    console.log(result);
  })
  .catch((error) => {
    console.log(error);
  });
```
There is also `.finally()` which gets executed regardless of whether the promise was a success or failure;
```js
let myPromise = new Promise(function (resolve, reject) {
  let x = 1;
  if (x === 1) {
    resolve("x is 1");
  } else {
    reject("x is not 1");
  }
});

myPromise
  .then((result) => {
    console.log(result);
  })
  .catch((error) => {
    console.log(error);
  })
  .finally(() => {
    console.log("It was nice working with this promise");
  });
  ```
  ## Returning a promise from a function
  ```js
  function fetchUser() {
  return new Promise(function (resolve, reject) {
    let error = false;
    if (error === true) {
      reject("There was an error");
    } else {
      resolve({ username: "_john", role: "Admin" });
    }
  });
}

fetchUser()
  .then((user) => {
    console.log(`Username: ${user.username}, Role: ${user.role}`);
  })
  .catch((error) => {
    console.log(error);
  });
```

























