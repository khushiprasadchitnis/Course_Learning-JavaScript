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

### Task 1
Create an HTML page with an inline JavaScript alert.
### Solution
```html
<button onclick="alert('Hello, JavaScript!')">Click Me</button>
```

### Task 2
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

### Task 3
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
