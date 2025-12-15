# Python Learning Assignment Documentation

This document provides detailed explanations of the Python programs in this learning directory.

---

## 1. Calculator.py

### Overview
A simple command-line calculator program that performs basic arithmetic operations (addition, subtraction, multiplication, and division) on two user-provided numbers.

### Code Structure

```python
a = int(input("Enter the first number: "))
b = int(input("Enter the second number: "))
print("\n")
if a and b:
    print("Addition: ", a+b)
    print("Subtraction: ", a-b)
    print("Multiplication: ", a*b)
    print("Division: ", a/b)
else:
    print("Two numbers are required")
```

### Functionality

#### Input
- **Line 1-2**: The program prompts the user to enter two numbers
  - Uses `input()` to get user input
  - Converts the input to integers using `int()`
  - Stores values in variables `a` and `b`

#### Processing
- **Line 3**: Prints a blank line for better readability
- **Line 4**: Checks if both `a` and `b` have values using a conditional statement
  - Note: This condition will always be `True` for non-zero integers, but `False` if either is `0`

#### Output
- **Lines 5-8**: If the condition is met, prints four arithmetic operations:
  - **Addition**: Sum of both numbers
  - **Subtraction**: Difference between first and second number
  - **Multiplication**: Product of both numbers
  - **Division**: Quotient when first number is divided by second
- **Line 10**: Displays error message if the condition fails

### Usage Example
```
Enter the first number: 10
Enter the second number: 5

Addition:  15
Subtraction:  5
Multiplication:  50
Division:  2.0
```

### Potential Improvements
- Handle division by zero error
- Add input validation for non-numeric inputs
- The condition `if a and b` evaluates to `False` when either number is `0`, which may not be the intended behavior
- Add more operations (modulus, exponentiation, etc.)

---

## 2. custom_greet.py

### Overview
A personalized greeting program that takes the user's first and last name as input and displays a custom welcome message.

### Code Structure

```python
firstname = input("Enter your first name: ")
lastname = input("Enter your last name: ")
print("Hello,", firstname, lastname+"!", "Welcome to the Python program.", sep=" ")
```

### Functionality

#### Input
- **Line 1**: Prompts user to enter their first name and stores it in `firstname` variable
- **Line 2**: Prompts user to enter their last name and stores it in `lastname` variable

#### Output
- **Line 3**: Constructs and displays a personalized greeting message
  - Uses the `print()` function with multiple arguments
  - **`sep=" "`**: Specifies that arguments should be separated by a single space
  - Concatenates `lastname` with `"!"` using the `+` operator
  - Combines all elements into: "Hello, [firstname] [lastname]! Welcome to the Python program."

### Usage Example
```
Enter your first name: John
Enter your last name: Doe
Hello, John Doe! Welcome to the Python program.
```

### Key Concepts Demonstrated
- **String Input**: Capturing text input from users
- **String Concatenation**: Using `+` operator to join strings
- **Print Parameters**: Using the `sep` parameter to control output formatting
- **Multiple Print Arguments**: Passing multiple values to `print()` function

### Potential Enhancements
- Add input validation to ensure names are not empty
- Capitalize names automatically using `.title()` or `.capitalize()`
- Add more personalization options (age, location, etc.)
- Format the greeting with different styles

---

## Learning Objectives

These programs demonstrate fundamental Python concepts:

1. **User Input**: Using `input()` function to interact with users
2. **Data Types**: Working with strings and integers
3. **Type Conversion**: Converting strings to integers using `int()`
4. **Conditional Statements**: Using `if-else` to control program flow
5. **Arithmetic Operations**: Performing basic mathematical calculations
6. **String Manipulation**: Concatenating and formatting strings
7. **Output Formatting**: Using `print()` function with various parameters

---

## Running the Programs

### Calculator
```bash
python Calculator.py
```

### Custom Greet
```bash
python custom_greet.py
```

---

*Last Updated: December 2025*
