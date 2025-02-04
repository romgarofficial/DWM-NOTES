# MODULE 1

![enter image description here](https://www.datocms-assets.com/48401/1628644950-javascript.png?auto=format&fit=max&w=1200)


# Session Content

 - Environment Check
 - What is JavaScript?
 - How to Start Coding With JavaScript
 - JS Variables
 - JS Data Types
 - JS Comments
 - JS Operators
	 - Arithmetic Operators
	 - Relational Operators
	 - Comparison Operators
	 - Logical Operators

## Objective

This session aims to provide a comprehensive introduction to JavaScript, starting with an environment check to ensure all participants are set up correctly. We will explore the fundamentals of JavaScript, including what it is and its significance in web development. Participants will learn about JavaScript variables, comments, and various operators, focusing on arithmetic, relational, comparison, and logical operators. By the end of the session, attendees will have a solid understanding of these core JavaScript concepts, enabling them to write and debug basic JavaScript code. This foundational knowledge will prepare participants for more advanced JavaScript topics in future sessions.

## Environment Check: Setting Up JavaScript Development

-   **Download Visual Studio Code**: Visit the Visual Studio Code download page and choose the version compatible with your operating system (Windows, macOS, or Linux). Follow the installation instructions to set it up on your computer.
	- [VS Code Download Page](https://code.visualstudio.com/download)
    
-   **Download Google Chrome**: Go to the Google Chrome download page and download the browser for your operating system. Follow the installation instructions to install Chrome on your computer.
	- [Download Google Chrome](https://www.google.com/intl/en_uk/chrome/?brand=CHBD&ds_kid=43700081225882217&gad_source=1&gclid=CjwKCAiA74G9BhAEEiwA8kNfpV6kqv7xQz3NNBanIbiHEDMppQfDI48KHuunT55zcNvW6yxgyHmcAxoCm8cQAvD_BwE&gclsrc=aw.ds)


## What is JavaScript?

JavaScript is crucial in data warehousing and management due to its versatility. It can automate ETL (Extract, Transform, Load) processes, making data extraction and transformation efficient. JavaScript's libraries like D3.js and Chart.js enable creating interactive data visualizations for better analysis. Its client-side capabilities facilitate the development of dashboards and user interfaces for data interaction. Additionally, with Node.js, JavaScript can manage server-side tasks and integrate with various APIs for seamless data access.

## How to Start Coding With JavaScript?

### Step 1: Create a New Folder
1. Open Visual Studio Code.
2. Create a new folder for your project. You can name it `myProject` or any name you prefer.
3. Open the folder in Visual Studio Code by going to `File > Open Folder` and selecting your newly created folder.

### Step 2: Create `index.html`
1. In Visual Studio Code, right-click on the folder and select `New File`.
2. Name the file `index.html`.
3. Open `index.html` and type `!` followed by pressing `Tab` to generate the basic HTML structure. It should look like this:
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
        
    </body>
    </html>
    ```

### Step 3: Create `index.js`
1. In Visual Studio Code, right-click on the folder and select `New File`.
2. Name the file `index.js`.

### Step 4: Link `index.js` to `index.html`
1. Open `index.html` and add a `<script>` tag within the `<body>` tags to link the JavaScript file:
    ```html
    <body>
        <!-- Your content here -->

        <script src="index.js"></script>
    </body>
    ```

### Step 5: Write JavaScript Code
1. Open `index.js` and write some simple JavaScript code. For example:
    ```javascript
    console.log('Hello, world!');
    ```

### Step 6: Open `index.html` in the Browser
1. In Visual Studio Code, right-click on `index.html` and select `Open with Live Server`. If you don't have the Live Server extension installed, you can install it from the Extensions Marketplace.
2. Your default web browser should open and display the content of `index.html`.

### Step 7: Open Developer Tools
1. Open Developer Tools in your web browser by pressing `F12` or right-clicking on the page and selecting `Inspect`.
2. Go to the `Console` tab to see the output of your JavaScript code.

You should see `Hello, world!` in the console, indicating that your HTML and JavaScript files are correctly linked and working together.


## JavaScript Variables

In programming, a variable is a container that holds a value. It's like a labeled box where you can store data, which you can then retrieve and manipulate later. Think of it as a way to give a name to a piece of information so you can use it throughout your code.

**`let` vs. `const`**

In JavaScript, there are different ways to declare variables, with `let` and `const` being two of the most common.

-   `let`: This keyword is used to declare variables that can be reassigned later. It's like having a changeable address label on a box. You can update the label to point to a different box if needed.
    
-   `const`: This keyword is used to declare variables that cannot be reassigned once they've been set. It's like a permanent marker on a box. Once you write on it, you can't change the label.

**Real-World Analogy**

Imagine you have two types of boxes:

-   **A cardboard box with a sticky note label**: You can easily remove the sticky note and put a new one with a different label. This is like a `let` variable where the contents can change.
    
-   **A wooden box with a permanent marker label**: Once you write on the box with a permanent marker, you can't change the label. This is like a `const` variable where the contents cannot change after being set.
- 
**Sample Code**
Here's some sample code to illustrate the difference between `let` and `const`:

```javascript
// Using let
let myAge = 25;    // Declare a variable with let
console.log(myAge); // Output: 25

myAge = 26;        // Reassign the variable
console.log(myAge); // Output: 26

// Using const
const birthYear = 1999;  // Declare a variable with const
console.log(birthYear);  // Output: 1999

// Trying to reassign a const variable will result in an error
// birthYear = 2000;      // Uncommenting this line will cause an error: TypeError: Assignment to constant variable.
```

## JavaScript Data Types

Data types are a fundamental concept in programming that define the type of data a variable can hold and the operations that can be performed on it. Different data types serve different purposes in a program, helping ensure that the right kind of data is used and processed correctly. Here are the main data types in JavaScript:

**Numbers**
Represents numerical data, including both integers and floating-point numbers.
```javascript
let age = 30;           // Integer
let pi = 3.14;          // Floating-point number
console.log(age);       // Output: 30
console.log(pi);        // Output: 3.14
```
**Strings**
Represents text data enclosed within quotes.
```javascript
let name = "John Doe";  // String
console.log(name);      // Output: John Doe
```

**Booleans**
Represents logical values: true or false.
```javascript
let isStudent = true;   // Boolean
let hasGraduated = false; // Boolean
console.log(isStudent); // Output: true
console.log(hasGraduated); // Output: false
```

**Arrays**
Represents a collection of elements, which can be of any data type, enclosed within square brackets.
```javascript
let fruits = ["apple", "banana", "cherry"]; // Array
console.log(fruits);   // Output: ["apple", "banana", "cherry"]
console.log(fruits[0]); // Output: apple
```

**Objects**
Represents a collection of properties, where each property is a key-value pair.
```javascript
let person = {
  name: "Jane Doe",
  age: 25,
  isStudent: false
}; // Object
console.log(person); // Output: { name: 'Jane Doe', age: 25, isStudent: false }
console.log(person.name); // Output: Jane Doe
```

## JavaScript Comment

Comments in JavaScript are used to leave notes or explanations within the code, which can help make the code more understandable for yourself and others who might read it. Comments are ignored by the JavaScript engine, so they have no effect on the actual execution of the code. There are two types of comments in JavaScript: single-line comments and multi-line comments.

**Single-Line Comments**
Single-line comments are created using `//`. Anything following `//` on that line will be considered a comment.

**Example:**
```javascript
// This is a single-line comment
let x = 5; // This is an inline comment
console.log(x); // Output: 5
```
**Multi-Line Comments**
Multi-line comments are created using `/*` to start the comment and `*/` to end it. Everything between these markers will be treated as a comment.

**Example:**
```javascript
/*
  This is a multi-line comment.
  It can span multiple lines.
*/
let y = 10;
console.log(y); // Output: 10
```

## JavaScript Operators

JavaScript operators are special symbols used to perform operations on operands (values and variables). There are several types of operators, each serving different purposes. Let's take a look at some of the main categories:

**1. Arithmetic Operators**
Arithmetic operators are used to perform mathematical calculations.
**Addition (**`+`**)**
```javascript
let sum = 5 + 3; 
console.log(sum); // 8
```

**Subtraction (**`-`**)**
```javascript
let difference = 5 - 3;
console.log(difference); // 2
```

**Multiplication (**`*`**)**
```javascript
let product = 5 * 3;
console.log(product); // 15
```

**Division (**`/`**)**
```javascript
let quotient = 5 / 3; 
console.log(quotient ); // 1.6666...
```

**Modulus (**`%`**)**
```javascript
let remainder = 5 % 3; 
console.log(remainder); // 2
```
The modulus operator (`%`) in JavaScript is used to find the remainder of a division between two numbers. It's a useful operator when you want to determine if a number is divisible by another number, or when you need to wrap around a range of values, such as in circular buffers or clock arithmetic.

**You can use arithmetic operators with reference values of variables as operands in JavaScript. This allows you to perform calculations using the values stored in variables.**

**Example**
Let's say we have two variables, `a` and `b`, and we want to perform various arithmetic operations on them.

```javascript
let a = 10;
let b = 5;

// Addition
let sum = a + b;
console.log(sum); // Output: 15

// Subtraction
let difference = a - b;
console.log(difference); // Output: 5

// Multiplication
let product = a * b;
console.log(product); // Output: 50

// Division
let quotient = a / b;
console.log(quotient); // Output: 2

// Modulus
let remainder = a % b;
console.log(remainder); // Output: 0

// Exponentiation
let power = a ** b;
console.log(power); // Output: 100000
```
In this example, `a` and `b` are used as operands for various arithmetic operations. The results are stored in new variables (`sum`, `difference`, `product`, `quotient`, `remainder`, and `power`) and then logged to the console.

Using variables as operands makes your code more flexible and readable, allowing you to easily change the values of `a` and `b` without modifying the operations themselves.

**2. Comparison Operators**
Comparison operators are used to compare two values and return a boolean result (`true` or `false`). Let's explore the `==`, `===`, `!=`, and `!==` operators in JavaScript with explanations and sample code.

**`==` (Equal To)**
The `==` operator checks if two values are equal, but it performs type coercion, meaning it converts the operands to the same type before making the comparison.

**Example:**

```javascript
let a = 5;
let b = '5';

console.log(a == b); // Output: true
```
In this example, `a` and `b` are considered equal because `==` converts the string `'5'` to the number `5` before comparing.

**`===` (Strict Equal To)**
The `===` operator checks if two values are equal and of the same type. It does not perform type coercion.

**Example:**

```javascript
let a = 5;
let b = '5';

console.log(a === b); // Output: false
```
Here, `a` and `b` are not considered equal because `a` is a number and `b` is a string, and `===` does not perform type conversion.

**`!=` (Not Equal To)**
The `!=` operator checks if two values are not equal, performing type coercion if necessary.

**Example:**

```javascript
let a = 5;
let b = '5';

console.log(a != b); // Output: false
```
In this case, `a` and `b` are considered equal due to type coercion, so `!=` returns `false`.

**`!==` (Strict Not Equal To)**
The `!==` operator checks if two values are not equal or not of the same type. It does not perform type coercion.

**Example:**

```javascript
let a = 5;
let b = '5';

console.log(a !== b); // Output: true
```
Here, `a` and `b` are not equal in terms of value and type, so `!==` returns `true`.

**Summary of Comparison Operators**

```javascript
let x = 5;
let y = '5';

console.log(x == y);  // true (type coercion)
console.log(x === y); // false (strict equality)
console.log(x != y);  // false (type coercion)
console.log(x !== y); // true (strict inequality)
```
Using these comparison operators appropriately helps ensure accurate comparisons and control flow in your JavaScript code.

**3. Relational Operators**
Explore the relational operators `<`, `>`, `<=`, and `>=`  in JavaScript. These operators are used to compare two values and return a boolean result (`true`  or `false`).

**`<` (Less Than)**
The `<` operator checks if the value on the left is less than the value on the right.

**Example:**

```javascript
let a = 5;
let b = 10;
console.log(a < b); // Output: true
```
In this example, `5` is less than `10`, so the result is `true`.

**`>` (Greater Than)**
The `>` operator checks if the value on the left is greater than the value on the right.

**Example:**

```javascript
let a = 15;
let b = 10;
console.log(a > b); // Output: true
```
Here, `15` is greater than `10`, so the result is `true`.

**`<=` (Less Than or Equal To)**
The `<=` operator checks if the value on the left is less than or equal to the value on the right.

**Example:**

```javascript
let a = 10;
let b = 10;
console.log(a <= b); // Output: true
```
In this case, `10` is equal to `10`, so the result is `true`.

**`>=` (Greater Than or Equal To)**
The `>=` operator checks if the value on the left is greater than or equal to the value on the right.

**Example:**

```javascript
let a = 20;
let b = 15;
console.log(a >= b); // Output: true
```
Here, `20` is greater than `15`, so the result is `true`.

**Summary of Relational Operators**

```javascript
let x = 5;
let y = 10;
let z = 5;

console.log(x < y);  // true
console.log(x > y);  // false
console.log(x <= z); // true
console.log(x >= z); // true
```
what about <, >, <=, >=

Sure, let's explore the relational operators `<`, `>`, `<=`, and `>=` in JavaScript. These operators are used to compare two values and return a boolean result (`true` or `false`).

 **`<` (Less Than)**

The `<` operator checks if the value on the left is less than the value on the right.

**Example:**



```javascript
let a = 5;
let b = 10;
console.log(a < b); // Output: true

```

In this example, `5` is less than `10`, so the result is `true`.

**`>` (Greater Than)**

The `>` operator checks if the value on the left is greater than the value on the right.

**Example:**



```javascript
let a = 15;
let b = 10;
console.log(a > b); // Output: true

```

Here, `15` is greater than `10`, so the result is `true`.

**`<=` (Less Than or Equal To)**

The `<=` operator checks if the value on the left is less than or equal to the value on the right.

**Example:**



```javascript
let a = 10;
let b = 10;
console.log(a <= b); // Output: true

```

In this case, `10` is equal to `10`, so the result is `true`.

 **`>=` (Greater Than or Equal To)**

The `>=` operator checks if the value on the left is greater than or equal to the value on the right.

**Example:**



```javascript
let a = 20;
let b = 15;
console.log(a >= b); // Output: true

```

Here, `20` is greater than `15`, so the result is `true`.

**Summary of Relational Operators**


```javascript
let x = 5;
let y = 10;
let z = 5;

console.log(x < y);  // true
console.log(x > y);  // false
console.log(x <= z); // true
console.log(x >= z); // true
```

These relational operators are essential for making comparisons and control flow decisions in your JavaScript code.

**3. Logical Operators**
Logical operators in JavaScript are used to combine or invert boolean values (`true` or `false`). They are particularly useful in control flow statements (like `if` conditions) where you need to evaluate multiple conditions.

**Logical AND (`&&`)**
The `&&` operator returns `true` if both operands are `true`. Otherwise, it returns `false`.

**Example:**

```javascript
let a = true;
let b = false;
let c = true;

console.log(a && b); // Output: false (because b is false)
console.log(a && c); // Output: true (because both a and c are true)
```

**Logical OR (`||`)**
The `||` operator returns `true` if at least one of the operands is `true`. If both operands are `false`, it returns `false`.

```javascript
let a = true;
let b = false;
let c = false;

console.log(a || b); // Output: true (because a is true)
console.log(b || c); // Output: false (because both b and c are false)
```

**Real-World Analogy**
Think of the logical operators like switches:

-   **AND (**`&&`**)**: Two switches need to be on for the light to turn on.
    
-   **OR (**`||`**)**: At least one switch needs to be on for the light to turn on.

```javascript
let x = true;
let y = false;

console.log(x && y); // false
console.log(x || y); // true
```
These logical operators are essential tools in JavaScript for evaluating and combining multiple conditions in your code.

## Helpful Links

 - [W3Schools JavaScript](https://www.w3schools.com/js/default.asp)
 - [W3Schools Intro to JavaScript](https://www.w3schools.com/js/js_intro.asp)
 - 
