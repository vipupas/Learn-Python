# Chapter 1: Getting Started with Python

## Table of Contents
1. [The Interactive Shell](#the-interactive-shell)
2. [Expressions](#expressions)
3. [Data Types](#data-types)
4. [String Values in Variables](#string-values-in-variables)
5. [Variable Naming](#variable-naming)
6. [Your First Program: Hello World](#your-first-program-hello-world)
7. [Script Mode](#script-mode)
8. [The print() Function](#the-print-function)
9. [The input() Function](#the-input-function)
10. [Built-in Functions](#built-in-functions)

---

## The Interactive Shell

The Python interactive shell (also called the Python interpreter or REPL - Read-Eval-Print Loop) is a powerful tool that allows you to execute Python code line by line and see immediate results.

### Starting the Interactive Shell

To start the Python interactive shell, open your terminal or command prompt and type:

```bash
python
```

or

```bash
python3
```

You'll see something like this:

```
Python 3.11.0 (main, Oct 24 2022, 18:26:48) [MSC v.1933 64 bit (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.
>>>
```

The `>>>` prompt indicates that Python is ready to accept your commands.

You can check version with `--version` flag .

### Using the Interactive Shell

You can type Python expressions and statements directly at the prompt:

```python
>>> 2 + 3 # use like calculator
5
>>> print("Hello, World!")
Hello, World!
>>> x = 10
>>> x * 2
20
```

To exit the interactive shell, type `exit()` or use `Ctrl+D` (Linux/Mac) or `Ctrl+Z` (Windows).

---

## Expressions

An expression is a combination of values, variables, operators, and function calls that Python can evaluate to produce a result.

### Basic Arithmetic Expressions / Operators

```python
>>> 5 + 3        # Addition
8
>>> 10 - 4       # Subtraction
6
>>> 6 * 7        # Multiplication
42
>>> 15 / 3       # Division
5.0
>>> 17 // 5      # Floor division
3
>>> 17 % 5       # Modulo (remainder)
2
>>> 2 ** 3       # Exponentiation
8
```

### Comparison Expressions / Operators

```python
>>> 5 > 3        # Greater than
True
>>> 10 == 10     # Equal to  { a = 1 this is assignment operator }
True
>>> 7 != 5       # Not equal to
True
>>> 4 <= 4       # Less than or equal to
True
>>> 4 >= 4       # greater than or equal to
True
```

### Assignment Expression / Operators
```python
>>> a = 10          # a is assign with 10
10
>>> a += 10         # a = a + 10
>>> a /= 10         # a = a / 10
>>> a //= 10        # a = a // 10
>>> a %= 10         # a = a % 10
>>> a *= 10         # a = a * 10
>>> a **= 3         # a = a ** 10
>>> a -= 10         # a = a - 10
```

### String Expressions

```python
>>> "Hello" + " World"    # String concatenation
'Hello World'
>>> "Python" * 3          # String repetition
'PythonPythonPython'
>>> "apple" < "banana"    # String comparison
True
```

---

## Data Types

Python has several built-in data types. The three fundamental types are : `int()`, `float()`, and `str()`.

### Integer

Integers are whole numbers without decimal points. They can be +ve, -ve, or 0.

```python
>>> 42
42
>>> -17
-17
>>> 0
0
>>> type(42)
<class 'int'>
```

### Floating Point

Floating-point numbers (floats) contain decimal points and can represent fractional values.

```python
>>> 3.14
3.14
>>> -2.5
-2.5
>>> 0.0
0.0
>>> type(3.14)
<class 'float'>
```

### String

Strings are sequences of characters enclosed in single quotes (`'`) or double quotes (`"`).

```python
>>> "Hello, World!"
'Hello, World!'
>>> 'Python Programming'
'Python Programming'

>>> type("Hello")
<class 'str'>
```

---

## String Values in Variables

Variables can store string values, making them reusable throughout your program.

### Assigning Strings to Variables

```python
>>> name = "Alice"
>>> greeting = "Hello, World!"
```

### String Operations with Variables

```python
>>> first_name = "John"
>>> last_name = "Doe"
>>> first_name + " " + last_name
John Doe

>>> "Hi! " * 3
Hi! Hi! Hi! 
```
---

## Variable Naming

Variables are containers for storing data values. Python has specific rules and conventions for naming variables.

### Variable Naming Rules

1. **Must start with a letter or underscore**: Variable names cannot start with a number.
2. **Can contain letters, numbers, and underscores**: No spaces or special characters.
3. **Case-sensitive**: `myVar` and `myvar` are different variables.
4. **Cannot use Python keywords**: Words like `if`, `for`, `class`, etc. are reserved.

### Valid Variable Names

```python
>>> name = "Alice"
>>> age = 25
>>> user_id = 12345
>>> _private_var = "secret"
>>> firstName = "John"
>>> PI = 3.14159
>>> var123 = "test"
```

### Invalid Variable Names

```python
# These will cause errors:
# 123name = "Alice"        # Cannot start with number
# user-id = 12345          # Cannot contain hyphen
# class = "MyClass"        # Cannot use Python keywords
# user name = "John"       # Cannot contain spaces
```

### Python Keywords (Reserved Words)

```python
False      await      else       import     pass
None       break      except     in         raise
True       class      finally    is         return
and        continue   for        lambda     try
as         def        from       nonlocal   while
assert     del        global     not        with
async      elif       if         or         yield
```

### Naming Conventions

1. **Use descriptive names**: `student_count` instead of `sc`
2. **Use snake_case**: `user_name` instead of `userName`
3. **camelCase**: this is `userName`
4. **Constants in UPPERCASE**: `MAX_SIZE = 100`
5. **Avoid single letters**: except for loop counters (`i`, `j`, `k`)

---

## Your First Program: Hello World

The "Hello, World!" program 

### In the Interactive Shell

```python
>>> print("Hello, World!")
Hello, World!
```

### Understanding the Program

The `print()` function displays the text inside the parentheses to the screen.

### Variations

```python
>>> print("Hello, Python!")
Hello, Python!
>>> print('Welcome to programming!')
Welcome to programming!
>>> print("Learning Python is fun!")
Learning Python is fun!
```
---

## Script Mode

While the interactive shell is great for testing small pieces of code, real programs are written in script mode using text files.

### Creating a Python Script

1. Create a new file with a `.py` extension (e.g., `hello.py`)
2. Write your Python code in the file
3. Save the file
4. Run it from the command line

### Running the Script

From the command line or terminal:

```bash
python3 hello.py
```

---

## The print() Function

The `print()` function is used to display output on the screen.

### Basic Usage

```python
>>> print("Hello, World!")
Hello, World!
>>> print(42)
42
>>> print(3.14)
3.14
```

### Printing Multiple Values

```python
>>> print("Name:", "Alice", "Age:", 25)
Name: Alice Age: 25
>>> print("The answer is", 42)
The answer is 42
```

### Customizing Output

```python
>>> print("Hello", "World", sep="-")
Hello-World
>>> print("Hello", "World", sep="")
HelloWorld
>>> print("Line 1", end=" ")
>>> print("Line 2")
Line 1 Line 2
```

### Printing Variables

```python
>>> name = "Bob"
>>> age = 30
>>> print("Name:", name)
Name: Bob
>>> print("Age:", age)
Age: 30
>>> print("Hello,", name, "! You are", age, "years old.")
Hello, Bob ! You are 30 years old.
```
---

### Comments in Scripts

Use the `#` symbol to add comments to your code.
This will not treat as part of code.

```python
# This is a comment
print("This code will run")  # instruction and explaination for programmer
```

---

## The input() Function

The `input()` function allows you to get user input from the keyboard.

### Basic Usage

```python
>>> name = input("What is your name? ")
What is your name? Alice
>>> print("Hello,", name)
Hello, Alice
```

### Important Notes

1. `input()` always returns a string
2. The prompt message is optional but recommended
3. The program waits for the user to press Enter

### Examples :

```python
favorite_color = input("What's your favorite color? ")
print("Your favorite color is", favorite_color)
age_str = input("How old are you? ")
print("You entered:", age_str)
print("Type of input:", type(age_str))
```

### Converting Input to Numbers

```python
>>> age_str = input("Enter your age: ")
Enter your age: 25
>>> age = int(age_str)
>>> print("Next year you'll be", age + 1)
Next year you'll be 26
```

---

## Built-in Functions

- Many built-in functions for common tasks. Here are the essential ones for beginners.

- Built-in function is like different shapes of Lego pieces.

### len() Function

Returns the length of a string, list, or other sequence.

```python
>>> len("Hello")
5
>>> len("Python Programming")
18
>>> word = "Computer"
>>> print("The word", word, "has", len(word), "letters")
The word Computer has 8 letters
```

### str() Function

Converts values to strings.

```python
>>> str(42)
'42'
>>> str(3.14)
'3.14'
>>> str(True)
'True'
>>> number = 100
>>> text = "The number is " + str(number)
>>> print(text)
The number is 100
```

### int() Function

Converts strings or numbers to integers.

```python
>>> int("42")
42
>>> int("123")
123
>>> int(3.14)
3
>>> int(3.99)    # Truncates, doesn't round
3
>>> age_str = "25"
>>> age = int(age_str)
>>> print(age + 5)
30
```

### float() Function

Converts strings or numbers to floating-point numbers.

```python
>>> float("3.14")
3.14
>>> float("42")
42.0
>>> float(10)
10.0
>>> price_str = "19.99"
>>> price = float(price_str)
>>> print(price * 2)
39.98
```

### type() Function

Returns the type of a value or variable.

```python
>>> type(42)
<class 'int'>
>>> type(3.14)
<class 'float'>
>>> type("Hello")
<class 'str'>
>>> type(True)
<class 'bool'>
>>> x = 10
>>> print(type(x))
<class 'int'>
```

### round() Function

Rounds a number to the nearest integer or to a specified number of decimal places.

```python
>>> round(3.14159)
3
>>> round(3.7)
4
>>> round(3.14159, 2)
3.14
>>> round(3.14159, 3)
3.142
>>> price = 19.99
>>> print("Rounded price:", round(price))
Rounded price: 20
```

### abs() Function

Returns the absolute value of a number.

```python
>>> abs(-5)
5
>>> abs(5)
5
>>> abs(-3.14)
3.14
>>> abs(0)
0
>>> temperature = -10
>>> print("Temperature magnitude:", abs(temperature))
Temperature magnitude: 10
```

---

## Practice Exercises

Try these exercises to reinforce your understanding:

### Exercise 1: Basic Calculations
```python
# Calculate the area of a rectangle
length = 10
width = 5
area = length * width
print("Area:", area)
```

### Exercise 2: User Input and Conversion
```python
# Get user's name and age
name = input("Enter your name: ")
age_str = input("Enter your age: ")
age = int(age_str)
print("Hello", name + "! You are", age, "years old.")
```

### Exercise 3: String Operations
```python
# Work with strings
first_name = input("Enter your first name: ")
last_name = input("Enter your last name: ")
full_name = first_name + " " + last_name
print("Full name:", full_name)
print("Length of full name:", len(full_name))
```

### Exercise 4: Type Conversions
```python
# Demonstrate type conversions
num_str = "42"
num_int = int(num_str)
num_float = float(num_str)
print("String:", num_str, "Type:", type(num_str))
print("Integer:", num_int, "Type:", type(num_int))
print("Float:", num_float, "Type:", type(num_float))
```

---

These fundamentals form the foundation for all Python programming. Practice using these concepts, and you'll be ready to move on to more advanced topics. 

learn more about builtin