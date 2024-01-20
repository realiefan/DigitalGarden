---
{"dg-publish":true,"permalink":"/projects/java-script-guide-for-beginners/"}
---

# JavaScript guide for beginners
#code
## Variables
Variables are used to store data values in JavaScript. They can hold various types of data.

### Declaration and Assignment
```javascript
let age; // Declaration
age = 30; // Assignment
```

### Data Types
JavaScript has several data types:
- **Primitive Data Types**: String, Number, Boolean, Null, Undefined, Symbol.
- **Reference Data Types**: Object, Array, Function.

## Operators
Operators perform operations on variables and values.

### Arithmetic Operators
```javascript
let x = 10;
let y = 5;
let sum = x + y; // Addition
let diff = x - y; // Subtraction
let product = x * y; // Multiplication
let quotient = x / y; // Division
let remainder = x % y; // Modulus
```

### Comparison Operators
```javascript
let a = 10;
let b = 5;
let isEqual = a === b; // Equality
let isNotEqual = a !== b; // Inequality
let isGreater = a > b; // Greater than
let isLess = a < b; // Less than
```

## Control Flow
Control flow statements determine the order in which code is executed.

### Conditional Statements
```javascript
let age = 18;
if (age >= 18) {
    console.log("You can vote!");
} else {
    console.log("You cannot vote yet.");
}
```

### Loops
```javascript
for (let i = 0; i < 5; i++) {
    console.log(i); // Prints 0 to 4
}
```

## Functions
Functions are blocks of reusable code that can be called with different inputs.

### Function Declaration
```javascript
function greet(name) {
    console.log(`Hello, ${name}!`);
}
greet("Alice"); // Hello, Alice!
```

### Function Expression
```javascript
const multiply = function(x, y) {
    return x * y;
};
let result = multiply(3, 4); // 12
```

## Objects
Objects are collections of key-value pairs.

### Object Creation
```javascript
let person = {
    firstName: "John",
    lastName: "Doe",
    age: 30
};
```

### Accessing Object Properties
```javascript
console.log(person.firstName); // John
console.log(person["lastName"]); // Doe
```

## Arrays
Arrays are ordered collections of values.

### Array Declaration
```javascript
let fruits = ["apple", "banana", "cherry"];
```

### Accessing Array Elements
```javascript
console.log(fruits[0]); // apple
console.log(fruits.length); // 3
```

## Asynchronous JavaScript
JavaScript can execute code asynchronously using callbacks, promises, and async/await.

### Using Promises
```javascript
const fetchData = () => {
    return new Promise((resolve, reject) => {
        setTimeout(() => {
            resolve("Data fetched successfully!");
        }, 2000);
    });
};

fetchData()
    .then(data => {
        console.log(data);
    })
    .catch(error => {
        console.error(error);
    });
```

## Event Handling
Event handling allows you to respond to user interactions.

### Event Listener
```javascript
document.getElementById("myButton").addEventListener("click", function() {
    alert("Button clicked!");
});
```

## DOM Manipulation
You can manipulate the Document Object Model (DOM) to change the content and structure of web pages.

### Changing Text Content
```javascript
document.getElementById("myParagraph").textContent = "New text content";
```

### Adding Elements
```javascript
let newElement = document.createElement("div");
newElement.textContent = "New element";
document.body.appendChild(newElement);
```

This documentation provides a foundation for working with JavaScript, covering variables, data types, operators, control flow, functions, objects, arrays, asynchronous JavaScript, event handling, and DOM manipulation. Real-life examples demonstrate how to apply these concepts in practice.