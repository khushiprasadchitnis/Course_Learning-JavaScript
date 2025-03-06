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

### Task 1
Create a button that changes the background color of the page when clicked.

### Solution
```html
<button onclick="changeBackground()">Change Background</button>

<script>
    function changeBackground() {
        document.body.style.backgroundColor = "lightblue";
    }
</script>
```

### Task 2
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
