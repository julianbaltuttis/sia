# Using Fat Arrow Functions in JavaScript

*As part of ES6, JavaScript introduced 'fat arrow' functions, a new way to declare and use functions with a more concise syntax. Not only do they make your code cleaner, but they also change the way `this` behaves. Let's delve into the world of fat arrow functions with a simple example.*

**Understanding Fat Arrow Functions:**

A fat arrow function is a more concise syntax for writing function expressions. They utilize the "fat arrow" (=>) operator to define the function. 

Here's the basic syntax for a fat arrow function:

```javascript
let functionName = (parameters) => {
    // function body
}
```

The parentheses `()` hold the input parameters, and the function's body is contained within the `{}` braces. The `=>` is the "fat arrow" that gives these functions their name.

**A Simple Example:**

Let's say we have a simple function that adds two numbers. Here's how we could write it using fat arrow syntax:

```javascript
let addNumbers = (num1, num2) => {
    return num1 + num2;
}

console.log(addNumbers(2, 3));  // Outputs: 5
```

In this example, `addNumbers` is a fat arrow function that takes two parameters, `num1` and `num2`, and returns their sum.

**Simplified Syntax for Single Parameter and Single Statement:**

If your function has only one parameter, you can leave out the parentheses:

```javascript
let square = num => {
    return num * num;
}

console.log(square(5));  // Outputs: 25
```

Also, if the function body consists of a single statement that returns a value, you can omit the `return` keyword and the `{}` braces:

```javascript
let square = num => num * num;

console.log(square(5));  // Outputs: 25
```

**Understanding the 'this' Keyword:**

Fat arrow functions don't bind their own `this` value. Instead, `this` is set to the surrounding (lexical) context. Traditional function expressions bind their own `this` value, which can cause unexpected behavior in certain contexts. This property makes fat arrow functions particularly useful when working with event handlers and methods that require `this` to refer to object properties.

Remember, ES6's fat arrow functions provide a shorter, more concise syntax to write function expressions. Happy coding!
