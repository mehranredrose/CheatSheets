# Python Cheat Sheet

Python is a versatile and powerful programming language that is widely used for web development, data analysis, artificial intelligence, and more. Below is a detailed cheat sheet to help you get started with Python.

## Basics

### Comments
Single-line comments start with `#`.

```python
# This is a single-line comment.
```

Multi-line comments can be created using triple quotes (`'''` or `"""`).

```python
"""
This is a multi-line
comment in Python.
"""
```

### Variables and Data Types
Python is dynamically typed, so you don't need to declare the type of a variable.

```python
# Integer
a = 5

# Float
b = 3.14

# String
c = "Hello, World!"

# List (array)
d = [1, 2, 3, 4]

# Tuple (immutable array)
e = (1, 2, 3)

# Dictionary (key-value pairs)
f = {"name": "John", "age": 30}

# Boolean
g = True
```

### Basic Operations

#### Arithmetic Operators
```python
+   # Addition
-   # Subtraction
*   # Multiplication
/   # Division
%   # Modulus (remainder)
**  # Exponentiation
//  # Floor Division
```

#### Comparison Operators
```python
==  # Equal to
!=  # Not equal to
>   # Greater than
<   # Less than
>=  # Greater than or equal to
<=  # Less than or equal to
```

## Control Structures

### Conditional Statements
```python
if x > y:
    print("x is greater than y")
elif x < y:
    print("x is less than y")
else:
    print("x is equal to y")
```

### Loops
#### For Loop
```python
for i in range(5):
    print(i)
```

#### While Loop
```python
i = 0
while i < 5:
    print(i)
    i += 1
```

## Functions

```python
def greet(name):
    return "Hello, " + name + "!"

print(greet("John"))
```

## Classes and Objects

```python
class Dog:
    def __init__(self, name):
        self.name = name

    def bark(self):
        return self.name + " says woof!"

dog1 = Dog("Buddy")
print(dog1.bark())
```

## File Handling

#### Reading a File
```python
with open('file.txt', 'r') as file:
    content = file.read()
    print(content)
```

#### Writing to a File
```python
with open('file.txt', 'w') as file:
    file.write("Hello, World!")
```

## Error Handling

```python
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero")
finally:
    print("This will always execute")
```

## Libraries and Modules

```python
import math

print(math.sqrt(16))
```

### Installing Libraries
You can install libraries using `pip`:

```bash
pip install requests
```

## Built-in Functions

- `len()`: Returns the length of an object.
- `type()`: Returns the type of an object.
- `str()`, `int()`, `float()`: Type conversion functions.

## Data Structures

### List Comprehensions
```python
squares = [x**2 for x in range(10)]
print(squares)
```

### Dictionaries and Sets
Dictionaries store key-value pairs, while sets store unique elements.
```python
# Dictionary
d = {"name": "John", "age": 30}
print(d["name"])

# Set
s = {1, 2, 3, 4, 5}
print(s)
```

## Modules and Packages

Create a module by creating a `.py` file. Create a package by adding an `__init__.py` file.

### Importing Modules
```python
import math

print(math.sqrt(16))
```

### Importing Functions from a Module
```python
from math import sqrt

print(sqrt(16))
```

## Advanced Features

### Decorators
Decorators are used to modify or extend the behavior of functions.

```python
def my_decorator(func):
    def wrapper():
        print("Something is happening before the function is called.")
        func()
        print("Something is happening after the function is called.")
    return wrapper

@my_decorator
def say_hello():
    print("Hello!")

say_hello()
```

### Generators
Generators allow you to create iterators.

```python
def my_generator():
    yield 1
    yield 2
    yield 3

for value in my_generator():
    print(value)
```

### Context Managers
Context managers are used for resource management and cleanup.

```python
with open('file.txt', 'r') as file:
    content = file.read()
    print(content)
```

This cheat sheet provides a comprehensive overview of Python syntax and features. By mastering these elements, you can effectively write robust and efficient Python code.

Happy coding!
```
