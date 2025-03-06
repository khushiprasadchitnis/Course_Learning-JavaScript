# **Short JavaScript Course (5 Lessons)**

This short JavaScript course introduces students to JavaScript fundamentals, including integrating JavaScript with HTML, adding interactivity, and covering basic concepts. Each lesson includes an introduction, examples, and exercises.

# **Lesson 1: Integrating JavaScript with HTML**

## **Introduction**
JavaScript is a programming language that runs in web browsers and allows you to create dynamic and interactive web pages. Before writing JavaScript, we need to understand how it integrates with HTML.

## **Examples**

**1. Inline JavaScript**

```html
<button onclick="alert('Hello, World!')">Click Me</button>
```


**2. Internal JavaScript**
```html
<html>
<head>
    <script>
        function greet() {
            alert("Welcome to JavaScript!");
        }
    </script>
</head>
<body>
    <button onclick="greet()">Click Me</button>
</body>
</html>
```

**3. External JavaScript**

```html
<html>
<head>
    <script src="script.js"></script>
</head>
<body>
    <button onclick="greet()">Click Me</button>
</body>
</html>
```

```js
function greet() {
    alert("Hello from an external script!");
}
```

### Exercises

### Task
Create an HTML page with an inline JavaScript alert.
### Solution
```html
<button onclick="alert('Hello, JavaScript!')">Click Me</button>
```

### Task
Write an internal script that displays an alert when a button is clicked.

### Solution
```
<html>
<head>
    <script>
        function showAlert() {
            alert("This is an internal script alert!");
        }
    </script>
</head>
<body>
    <button onclick="showAlert()">Click Me</button>
</body>
</html>
```

### Task
Link an external JavaScript file to an HTML page and trigger a function on a button click.

### Solution
<html>
<head>
    <script src="script.js"></script>
</head>
<body>
    <button onclick="showAlert()">Click Me</button>
</body>
</html>

```js
function showAlert() {
    alert("Hello from the external JavaScript file!");
}
```

# Lesson 2: Interactivity with Buttons and Forms

## Introduction

JavaScript allows you to add interactivity to your web pages, such as handling button clicks and processing form inputs.

## Examples

1. Changing Text with JavaScript

```html
<p id="text">Hello!</p>
<button onclick="changeText()">Change Text</button>

<script>
    function changeText() {
        document.getElementById("text").innerHTML = "Text Changed!";
    }
</script>
```

2. Handling Form Input

```html
<input type="text" id="name" placeholder="Enter your name">
<button onclick="showName()">Submit</button>
<p id="output"></p>

<script>
    function showName() {
        let name = document.getElementById("name").value;
        document.getElementById("output").innerText = "Hello, " + name + "!";
    }
</script>

```

## Exercises

### Tasks
Create a button that changes the background color of the page when clicked.

### Solutions
```html
<button onclick="changeBackground()">Change Background</button>

<script>
    function changeBackground() {
        document.body.style.backgroundColor = "lightblue";
    }
</script>
```

### Task
Build a simple form that collects a user’s name and displays it when they click a button.

### Solution

```
<input type="text" id="userName" placeholder="Enter your name">
<button onclick="displayMessage()">Submit</button>
<p id="message"></p>

<script>
    function displayMessage() {
        let name = document.getElementById("userName").value;
        document.getElementById("message").innerText = "Hello, " + name + "!";
    }
</script>
```

# Lesson 3: JavaScript Variables, Data Types, and Operators

## Introduction

JavaScript uses variables to store data. These variables can hold different data types, and you can manipulate them using operators.

## Examples


1. Declaring Variables

```js
let name = "Alice"; // String
let age = 25; // Number
let isStudent = true; // Boolean

console.log(name, age, isStudent);
```

2. Basic Operators

```js
let x = 10;
let y = 5;
console.log(x + y); // 15
console.log(x - y); // 5
console.log(x * y); // 50
console.log(x / y); // 2
console.log(x % y); // 0
```

## Exercises

### Task
Declare a variable message and assign a string value to it. Print it in the console.

### Solutions
```
let message = "Welcome to JavaScript!";
console.log(message);
```

### Task
Write a JavaScript program that takes two numbers, adds them, and displays the result.

### Solutions
```
let num1 = 10;
let num2 = 20;
let sum = num1 + num2;
console.log("The sum is: " + sum);
```

# Lesson 4: Conditional Statements and Loops

## Introduction

JavaScript allows decision-making using if, else, and switch statements. Loops help execute repeated tasks.

## Examples

1. If-Else Statements

```js
let age = 18;
if (age >= 18) {
    console.log("You are an adult.");
} else {
    console.log("You are a minor.");
}
```

2. For Loop
```js
for (let i = 0; i < 5; i++) {
    console.log("Iteration: " + i);
}
```

3. While Loop

```js
let count = 0;
while (count < 3) {
    console.log("Count is: " + count);
    count++;
}
```

## Exercises

### Task
Write a JavaScript program that checks whether a given number is positive or negative.

### Solutions
```
let number = -5;

if (number > 0) {
    console.log("The number is positive.");
} else if (number < 0) {
    console.log("The number is negative.");
} else {
    console.log("The number is zero.");
}
```

### Task
Create a loop that prints numbers from 1 to 10.

### Solutions
```
for (let i = 1; i <= 10; i++) {
    console.log(i);
}
```

# Lesson 5: Functions and Events

## Introduction

Functions allow you to write reusable blocks of code, and events enable interaction between the user and the web page.

## Examples

1. Defining a Function

```js
function greetUser(name) {
    return "Hello, " + name + "!";
}

console.log(greetUser("Alice"));
```

2. Event Listener

```html
<button id="myButton">Click Me</button>

<script>
    document.getElementById("myButton").addEventListener("click", function() {
        alert("Button was clicked!");
    });
</script>
```

## Exercises

### Task
Write a function that takes a number as input and returns its square.

### Solution
```
function square(num) {
    return num * num;
}
```

### Task
Add an event listener to a button that changes the color of a paragraph when clicked.

### Solution

```
<p id="text">Click the button to change my color!</p>
<button id="colorButton">Change Color</button>

<script>
    document.getElementById("colorButton").addEventListener("click", function() {
        document.getElementById("text").style.color = "red";
    });
</script>
```
