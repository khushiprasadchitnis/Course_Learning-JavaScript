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
