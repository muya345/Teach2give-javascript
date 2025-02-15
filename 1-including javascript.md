# INTRODUCTION OF JAVASCRIPT TO HTML
There are two main ways:
internal javascript
external JavaScript
## Internal
Javascript is written inside a `<script>` within the html file. Whereby placing the scripts at the bottom of the `<body>` element improves the display speed since script interpretation slows down display


```html 
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <h1>JavaScript</h1>
    <script>
      console.log("Hello, world!");
      console.log("JavaScript is fun")
    </script>
  </body>
</html>
```
## External 
Here javacript is stored in a separate `.js` file and linked to the HTML document using the `<script>` tag with a src attribute
```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <script src="app.js"></script>
  </head>
  <body>
    <h1>JavaScript</h1>
  </body>
</html
```
# Optimizing script loading
Javascript can block page rendering if not loaded correctly.
The browser sends a request to the server when the html code is parsed line by line  to download the resource
When it comes across the script tags to download JavaScript, it stops until the JavaScript has been downloaded, it then executes this JavaScript after it has been downloaded and then continues parsing the HTML which can end up hurting performance.
You can use the following to improve performance:
1. `defer` keyword which ensures that scrips are loade after the HTML is fully loaded.Eg
```html
<script src="app.js" defer></script> 
```
2. The `async` keyword which loads asynchronously and runs them as soon as they are downloaded and may execute javascript out of order.
```html
<script src="script.js" async></script>
```
3. The script tag or  tag at the end of the page 
- put the script tag at the very end of the page before the closing body tag.
```html
...
    <script src="app.js"></script>
</body>
</html>
```











