# Calculator


A simple Java-based calculator application that supports basic arithmetic operations: addition, subtraction, multiplication, and division. The application reads user input from the console and displays the result of the chosen operation.

## Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Project Structure](#project-structure)
- [Functions and Methods](#functions-and-methods)
- [Compilation and Execution](#compilation-and-execution)
- [Usage](#usage)
- [Sample Run](#sample-run)
- [Error Handling](#error-handling)
- [Author](#author)

## Features

- Addition of two integers
- Subtraction of two integers
- Multiplication of two integers
- Division of two integers (with division-by-zero check)

## Prerequisites

- Java Development Kit (JDK) 8 or higher
- A terminal or command prompt

## Project Structure

```
calculator-app/
├── src/
│   ├── Main.java
│   ├── Calculator.java
│   └── UserInput.java
└── README.md
```

- **Main.java**: Entry point of the application. Creates an instance of the `Calculator` and displays the result.
- **Calculator.java**: Contains the `Calculator` class with the `calculate` method that performs the arithmetic operations.
- **UserInput.java**: Handles user interaction and input collection via the console.

## Functions and Methods

### `class Calculator`

- **Method:** `public int calculate()`
  - Description: Handles the main logic of the calculator. It asks the user for input through the `UserInput` class, retrieves the operation choice and numbers, performs the corresponding arithmetic operation based on the choice, and returns the result.
  - Operations:
    - Addition (`choice == 1`)
    - Subtraction (`choice == 2`)
    - Multiplication (`choice == 3`)
    - Division (`choice == 4`)
    - Handles invalid choices and division by zero.

### `class UserInput`

- **Method:** `Object[] userInput()`
  - Description: Responsible for collecting user input from the console. Prompts the user to select an operation and input two numbers.
  - Returns: An `Object[]` array where the first element is the user's choice (integer) and the second element is an array of two integers (the numbers to be used in the operation).

### `class Main`

- **Method:** `public static void main(String[] args)`
  - Description: Entry point of the program. Creates an object of the `Calculator` class and calls its `calculate()` method. Prints the result to the console.



