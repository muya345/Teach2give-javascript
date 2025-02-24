# Introduction to `fetch` and HTTP Requests
`fetch` is a built-in JavaScript function that allows your code to communicate with other computers (servers) over the internet.

It helps your code send and receive data from websites or APIs (Application Programming Interfaces).

Think of it like asking a friend for information:

- You ask: "Hey, what is the weather today"

- They respond: "It’s sunny and 25°C."

Similarly, fetch sends a request to a website (server), and the server responds with some data.
## HTTP Request
HTTP (HyperText Transfer Protocol) is how computers communicate over the web.

There are different types of requests:

- GET: a computer asks for data (e.g., "Give me a list of users").

- POST: a computer sends data to be created on the server (e.g., "Create a new user, here are the details...").

- PUT: a computer requests for data updates (e.g., "Change the first name of John to Jack")

- DELETE: a computer requests for data to be deleted (e.g., "Delete information about John")

## Making a simple fetch request
We'll use jsonplaceholder.typicode.com, which gives fake user data.
```js
fetch("https://jsonplaceholder.typicode.com/users")
  .then(function (response) {
    return response.json();
  })
  .then(function (data) {
    console.log(data);
  })
  .catch(function (error) {
    console.log("There was an error");
    console.log(error);
  });
```
Explanation:

`fetch("https://jsonplaceholder.typicode.com/users/1")` Asks the server for user data (GET request).


```js
.then(function (response) {
  return response.json();
})
```
The response comes back, but not readable yet, so we convert it to JSON (a format that our computer can understand).

```js
.then(function (data) {
  console.log(data);
})
```
Receives data from the previous step and displays it in the user's console.

```js
.catch(function (error) {
  console.log("There was an error");
  console.log(error);
})
```
## Using async await for easier syntax
```js
async function fetchUser() {
  try {
    const response = await fetch(
      "https://jsonplaceholder.typicode.com/users/1",
    );
    const data = await response.json(); // Convert response to JSON
    console.log(data); // Display user data
  } catch (error) {
    console.error("Error:", error); // Handle errors
  }
}

fetchUser();
```
## Handling Errors
Sometimes, things go wrong (e.g., no internet, server issues). You should always handle errors:
```js
async function fetchUser() {
  try {
    const response = await fetch(
      "https://jsonplaceholder.typicode.com/users/1",
    );
    if (!response.ok) {
      console.log("Something went wrong");
      return;
    }
    const data = await response.json(); // Convert response to JSON
    console.log(data); // Display user data
  } catch (error) {
    console.error("Error:", error); // Handle errors
  }
}

fetchUser();
```

















