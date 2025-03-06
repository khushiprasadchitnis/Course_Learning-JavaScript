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

### Solution
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

### Solution
```
for (let i = 1; i <= 10; i++) {
    console.log(i);
}
```

