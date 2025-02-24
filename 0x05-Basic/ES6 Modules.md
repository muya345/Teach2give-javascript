# ES6 Modules
## Important Note About ES6 Modules﻿
If you are using ES6 Modules in a browser, you need to add `type="module"` in the `<script>` tag, for example:
```js
<script type="module" src="main.js"></script>
```
To use ES6 modules in Node.js:

Add `"type": "module"` in `package.json.`

Use `.mjs` file extensions.

## Exporting and Importing in ES6 Modules
You can export code from a module using either named exports or default exports.


## Named Exports
File: mathUtils.m
```js
export function add(1, 2) {
  return 1 + 2;
}

export function subtract(1, 2) {
  return 1 - 2;
}

export function multiply(1, 2) {
  return 1 * 2;
}
```
You can then import them in another module using the `import` keyword.

File: index.mjs
```js
import { add, subtract, multiply } from "./mathUtils.mjs";
console.log(add(5, 4));
console.log(subtract(5, 4));
console.log(multiply(5, 4));
```
Note: you must precede the file name with `./` when importing
### Using aliases for imports
```js
You can rename imports using the `as` keyword.
import { add as sum, subtract as difference, multiply } from "./mathUtils.mjs";
console.log(sum(5, 4));
console.log(difference(5, 4));
console.log(multiply(5, 4));
```
### Importing everything (`*` as an object)
You can import all named exports as a single object:
```js
import * as MathUtils from "./mathUtils.mjs";
console.log(MathUtils.add(5, 4));
console.log(MathUtils.subtract(5, 4));
console.log(MathUtils.multiply(5, 4));
```
## Default Exports﻿
Each module can have one default export, which can be imported with any name.

File: logger.mjs
```js
export default function log(message) {
  console.log(`Log: ${message}`);
}
```
Default exports don't need curly braces `{}` when importing.

You can import a default export with any name.

File: index.mjs
```js
import log from "./logger.mjs";

log("Hello, World");
```
