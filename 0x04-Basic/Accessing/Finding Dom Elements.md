# Accessing/Finding Dom Elements
To access any element in an HTML page, we first start by accessing the `document` object.
## Methods for accessing DOM elements
 ## `document.getElementById(elementId)`
 ```js
 <button id="my-button">Click Me</button>
 ```
 ```js
 const button = document.getElementById("my-button");
console.log(button); // <button id="my-button">Click Me</button>
```
### `document.getElementsByTagName(name)`
Finds all the elements that match the tag name passed, e.g., finding all paragraph elements in a page.

It returns a NodeList of all elements that match the tag name passed.
```js
<p>Hello, World</p>
<p>I love javascript   </p>
<p>JavaScript is great</p>
```
```js
<p>Hello, World</p>
<p>i love javascript</p>
<p>JavaScript is great</p>
```
#### `document.getElementsByClassName(className)`
Finds and returns a NodeList of all HTML elements with class attribute similar to the class specified.
```js
<p class="text">Hello, World</p>
<p class="text">I love JavaScript</p>
<p>JavaScript is great</p>
```
```js
const texts = document.getElementsByClassName("text");
console.log(texts); // [p.text, p.text]
```
### `document.querySelector(selector)```
Selects the first element in the document that matches a specified CSS selector, id or tag name.
```js
<p class="text">Hello, World</p>
<p class="text">I love JavaScript</p>
<p>JavaScript is great</p>
```
```js
const firstText = document.querySelector(".text");
console.log(firstText);
```
### `document.querySelectorAll(selector)`
Selects all elements in the document that match the specified class, id or tag name and returns a node list of them.
```js
<p class="text">Hello, World</p>
<p class="text">I love JavaScript</p>
<p>JavaScript is great</p>
```
```js
const paragraphs = document.querySelectorAll('p');
console.log(paragraphs); // [p.text, p.text, p]
```












