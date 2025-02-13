# MODULE 2

![enter image description here](https://camo.githubusercontent.com/e8fb88c8933205ec676a4baf05ac09bd8aa6e8c8a13c0f78c58f7b2917618e89/68747470733a2f2f7777772e6461746f636d732d6173736574732e636f6d2f34383430312f313632383634343935302d6a6176617363726970742e706e673f6175746f3d666f726d6174266669743d6d617826773d31323030)


# Session Content

 - JavaScript Dialog Methods
	 - Alert Method
	 - Prompt Method
 - Selection Control Structures
	 - If, Else If, Else Statement
	 - Switch-Case Statement
 - Repetition Control Structure
	 - Iterators
	 - While Loop
	 - While Loop with Prompt and Conditional Statement

## Objective
By the end of this lesson, students will have a comprehensive understanding of JavaScript's selection control structures, such as if-else-if and switch-case statements, enabling them to make decisions within their programs. Students will also master repetition control structures like for, while, and do-while loops, which allow efficient handling of repetitive tasks. Additionally, they will be able to effectively use JavaScript dialog methods, including alert, prompt, and confirm, to interact with users and gather input. Through practical examples and exercises, students will appreciate the importance of these control structures and dialog methods in creating dynamic and responsive web applications. This foundational knowledge will equip them with the skills to build more complex and user-friendly programs in JavaScript.



# JavaScript Dialog Methods
JavaScript Dialog Methods are built-in functions that allow you to interact with users through dialog boxes. They are simple, yet powerful tools for user interaction and input gathering.

## 1. Alert Method
Alerts are used to display messages to users. They are a simple way to inform the user about something important or provide feedback. The `alert()` method shows an alert box with a specified message and an OK button.

**Syntax:**
```javascript
alert(message);
```

**Example:**

```javascript
alert("Hello");
```
**Sample Output:**
![enter image description here](https://miro.medium.com/v2/resize:fit:1366/1*QpaoE2OwA1-uRV_8XrZcPg.png)
In this example, an alert box with the message "Hello! This is an alert message." will appear, and the user will need to click the OK button to close it.

## 2. Prompt Method
Alerts are used to display messages to users. They are a simple way to inform the user about something important or provide feedback. The `alert()` method shows an alert box with a specified message and an OK button.

**Syntax:**
```javascript
prompt(message);
```

**Example:**

```javascript
let userName = prompt("What is your name?");
alert("Hello, " + userName + "!");
```

![enter image description here](https://www.dummies.com/wp-content/uploads/492051.image0.jpg)
Once the user enters a name and clicks OK, an alert box will greet the user by name.

# JavaScript Selection Control Structures
JavaScript Selection Control Structures are programming constructs that allow you to make decisions in your code based on conditions. They enable the execution of different code blocks based on the evaluation of these conditions. The two primary selection control structures in JavaScript are the `if-else-if` and `switch-case` statements.

## 1. If-Else-If and Else
The `if-else` statement evaluates a condition. If the condition is true, it executes a specific block of code; if false, it executes another block of code. The `else-if` statement allows for multiple conditions to be checked sequentially.

**Syntax:**

```javascript
if (condition1) {
  // code to be executed if condition1 is true
} else if (condition2) {
  // code to be executed if condition2 is true
} else {
  // code to be executed if all conditions are false
}
```

**Example:**

```javascript
let age = 20;

if (age < 13) {
  console.log("You are a child.");
} else if (age < 20) {
  console.log("You are a teenager.");
} else {
  console.log("You are an adult.");
}
```
In this example, the program determines the user's age category by evaluating different conditions.

## 2. Switch-Case
The `switch` statement evaluates an expression and matches the expression's value against multiple cases. Each case is a possible value for the expression, and the corresponding code block is executed if there's a match.

**Syntax:**

```javascript
switch(expression) {
  case value1:
    // code to be executed if expression === value1
    break;
  case value2:
    // code to be executed if expression === value2
    break;
  // more cases
  default:
    // code to be executed if none of the cases match
}
```

**Example:**

```javascript
let day = 3;
let dayName;

switch (day) {
  case 1:
    dayName = "Sunday";
    break;
  case 2:
    dayName = "Monday";
    break;
  case 3:
    dayName = "Tuesday";
    break;
  case 4:
    dayName = "Wednesday";
    break;
  case 5:
    dayName = "Thursday";
    break;
  case 6:
    dayName = "Friday";
    break;
  case 7:
    dayName = "Saturday";
    break;
  default:
    dayName = "Invalid day";
}

console.log(dayName);
```

**Comparison**
-   **If-Else-If and Else**: Used for evaluating multiple conditions in a sequential manner.
    
-   **Switch-Case**: Used for matching an expression's value against multiple possible values, providing a cleaner way to handle discrete values.

# JavaScript Repetition Control Structures
JavaScript Repetition Control Structures, also known as loops, allow you to execute a block of code multiple times. These structures are useful for performing repetitive tasks efficiently. There are three main types of loops in JavaScript: `for`, `while`, and `do-while`.

## Iterators (Incrementation and Decrementation)

Incrementation and decrementation are fundamental concepts in programming that involve increasing or decreasing the value of a variable, respectively. These operations are particularly useful in loops and other repetitive tasks.

**Incrementation**
Incrementation refers to increasing the value of a variable by a certain amount, typically by one. The most common way to increment a variable in JavaScript is by using the increment operator (`++`).

**Example:**

```javascript
let count = 0;
count++; // count is now 1
count++; // count is now 2
console.log(count); // Output: 2
```

In this example, the variable `count` is incremented by 1 each time the `count++` statement is executed.

**Decrementation**
Decrementation refers to decreasing the value of a variable by a certain amount, typically by one. The most common way to decrement a variable in JavaScript is by using the decrement operator (`--`).

**Example:**

```javascript
let count = 5;
count--; // count is now 4
count--; // count is now 3
console.log(count); // Output: 3
```

In this example, the variable `count` is decremented by 1 each time the `count--` statement is executed.



## 1. While Loop
The `while` loop executes a block of code as long as a specified condition is true. The condition is checked before the loop is executed.

**Syntax:**

```javascript
while (condition) {
  // code to be executed
  //iterator
}
```

**Example:**

```javascript
let i = 0;

while (i < 5) {
  console.log("The number is " + i);
  i++;
}
```

**Output in the console:**
```javascript
//The number is 0
//The number is 1
//The number is 2
//The number is 3
//The number is 4
```

In this example, the loop runs as long as `i` is less than 5, printing the current value of `i` each time and incrementing `i`.

## While Loop with Prompt Method  and Conditional Statement

**Example:**
```javascript
let correctNumber = 7;
let userGuess = Number(prompt("Guess the number (between 1 and 10):"));

while (userGuess !== correctNumber) {
  if (userGuess < correctNumber) {
    userGuess = Number(prompt("Too low! Try again:"));
  } else if (userGuess > correctNumber) {
    userGuess = Number(prompt("Too high! Try again:"));
  }
}
alert("Congratulations! You guessed the correct number.");
```
**Explanation:**
-   **Initialize the correct number:** The variable `correctNumber` is set to 7, which is the number the user needs to guess.
    
-   **Prompt the user for a guess:** The `prompt()` method is used to ask the user to guess a number. The user's input is converted to an integer or number using `Number()` and stored in the variable `userGuess`.
    
-   **While loop:** The `while` loop continues to run as long as the user's guess (`userGuess`) is not equal to the correct number (`correctNumber`).
    
-   **Conditional checks within the loop:**
    
    -   If the user's guess is less than the correct number, a new prompt asks the user to guess again, stating that their guess was too low.
        
    -   If the user's guess is greater than the correct number, a new prompt asks the user to guess again, stating that their guess was too high.
        
-   **Congratulate the user:** Once the user guesses the correct number, the loop exits, and an alert message congratulates the user.

## Helpful Links

 - [W3School If, Else If, Else Statement](https://www.w3schools.com/js/js_if_else.asp)
 - [W3School Switch Case Statement](https://www.w3schools.com/js/js_switch.asp)
 - [W3School While Loop](https://www.w3schools.com/js/js_loop_while.asp)