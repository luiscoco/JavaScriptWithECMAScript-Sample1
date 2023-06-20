# JavaScript with ECMAScript. Sample1

To create and run a JavaScript application with ECMAScript modules (ES modules) in VSCode, you can follow these steps:

## 1.Set up a new project folder: 

Create a new folder on your computer where you want to store your project files.

## 2.Initialize a new project: 

Open the terminal in VSCode (View -> Terminal) and navigate to the project folder.

## 3.Use the following command to initialize a new project with npm (Node Package Manager):
```
npm init -y
```
This will create a package.json file in your project folder.

## 4.Install a development server: 

Since ES modules use module loading, you need to run your application on a development server. One popular option is using live-server. Install it by running the following command in the terminal:
```
npm install live-server --save-dev
```
## 5.Create an HTML file (index.html) 

Create an HTML file in your project folder, e.g., index.html. Open the file in VSCode and add the following code:

```html
<!DOCTYPE html>
<html>

<head>
    <title>ES Modules Example</title>
    <script src="main.js" type="module"></script>
</head>

<body>
    <h1>ES Modules Example</h1>
</body>

</html>
```

This code includes the main JavaScript file main.js as an ES module.

## 6.Create a JavaScript module(main.js) 

Create a new JavaScript file in your project folder, e.g., main.js.

Open the file in VSCode and add the following code:

```javascript
import { greet } from './greeting.js';
greet('John');
```
This code exports a function named greet and imports it from another module named greeting.js.

## 7.Create another JavaScript module(greeting.js)

Create a new JavaScript file in your project folder, e.g., greeting.js. 

Open the file in VSCode and add the following code:

```javascript
export function greet(name) {
  console.log(`Hello, ${name}!`);
}
```
