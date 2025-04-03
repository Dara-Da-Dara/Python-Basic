# Introduction to Python - 

## Course Overview
This introductory course covers the fundamentals of Python programming, guiding beginners through essential concepts and practical applications.

---

## Class 1: Getting Started with Python
### Topics Covered:
- Introduction to Python and its applications
- Installing Python and setting up the development environment
- Writing and running Python scripts
- Python syntax, indentation, and comments

### Theory:
Python is an interpreted, high-level programming language known for its readability and simplicity. It is widely used in web development, data science, automation, and AI.

### Hands-on Practice:
#### Running Python in interactive mode:
```python
>>> print("Hello, World!")
Hello, World!
```
# 🐍 Python Data Types

## 📌 Introduction
In Python, **data types** define the type of data a variable can hold. Understanding data types is fundamental for effective programming and data manipulation.

## 📝 Built-in Data Types
Python has several built-in data types, categorized as follows:

### 1️⃣ **Numeric Types**
Used for numerical operations.
- **`int`** – Integer values (e.g., `10`, `-5`)
- **`float`** – Floating-point numbers (e.g., `3.14`, `-0.5`)
- **`complex`** – Complex numbers (e.g., `3 + 4j`)

### 2️⃣ **Text Type**
- **`str`** – String type for textual data (e.g., `'Hello'`, `"Python"`)

### 3️⃣ **Sequence Types**
Used to store multiple items in a single variable.

# Mutable and Immutable Data in Python

## Mutable Data Types
Mutable objects can be changed after they are created. Operations on these objects can modify their contents without changing their identity (memory address).

### Examples:
- **Lists (`list`)**
- **Dictionaries (`dict`)**
- **Sets (`set`)**
- **Byte Arrays (`bytearray`)**

#### Example:
```python
my_list = [1, 2, 3]
print(id(my_list))  # Memory address before modification
my_list.append(4)
print(id(my_list))  # Same memory address after modification

- **`list`** – Ordered, mutable collection (e.g., `[1, 2, 3]`)
- **`tuple`** – Ordered, immutable collection (e.g., `(1, 2, 3)`)
- **`range`** – Immutable sequence of numbers (e.g., `range(5) → 0,1,2,3,4`)

### 4️⃣ **Set Types**
Used for storing unique elements.
- **`set`** – Unordered collection of unique elements (e.g., `{1, 2, 3}`)
- **`frozenset`** – Immutable version of a set

### 5️⃣ **Mapping Type**
- **`dict`** – Key-value pairs (e.g., `{'name': 'Alice', 'age': 25}`)

### 6️⃣ **Boolean Type**
- **`bool`** – Represents `True` or `False`

### 7️⃣ **Binary Types**
- **`bytes`** – Immutable sequence of bytes
- **`bytearray`** – Mutable sequence of bytes
- **`memoryview`** – Memory-efficient view of binary data

## 🔎 Checking Data Types
Use the `type()` function to check the type of a variable:
```python
x = 10
print(type(x))  # Output: <class 'int'>
```

## 🔄 Type Conversion (Type Casting)
Convert one data type to another using built-in functions:
```python
x = 5  # int
y = float(x)  # Convert int to float
z = str(x)  # Convert int to string
```

## 🚀 Summary
| Category    | Data Types |
|------------|-----------|
| Numeric    | `int`, `float`, `complex` |
| Text       | `str` |
| Sequence   | `list`, `tuple`, `range` |
| Set        | `set`, `frozenset` |
| Mapping    | `dict` |
| Boolean    | `bool` |
| Binary     | `bytes`, `bytearray`, `memoryview` |

Understanding these data types is crucial for working with Python efficiently. Happy Coding! 🚀

```
# Python Data Types

## 📌 Introduction
In Python, **data types** define the type of data a variable can hold. Understanding data types is fundamental for effective programming and data manipulation.

## 📝 Built-in Data Types
Python has several built-in data types, categorized as follows:

### 1️⃣ **Numeric Types**
Used for numerical operations.
- **`int`** – Integer values (e.g., `10`, `-5`)
- **`float`** – Floating-point numbers (e.g., `3.14`, `-0.5`)
- **`complex`** – Complex numbers (e.g., `3 + 4j`)

### 2️⃣ **Text Type**
- **`str`** – String type for textual data (e.g., `'Hello'`, `"Python"`)

### 3️⃣ **Sequence Types**
Used to store multiple items in a single variable.
- **`list`** – Ordered, mutable collection (e.g., `[1, 2, 3]`)
- **`tuple`** – Ordered, immutable collection (e.g., `(1, 2, 3)`)
- **`range`** – Immutable sequence of numbers (e.g., `range(5) → 0,1,2,3,4`)

### 4️⃣ **Set Types**
Used for storing unique elements.
- **`set`** – Unordered collection of unique elements (e.g., `{1, 2, 3}`)
- **`frozenset`** – Immutable version of a set

### 5️⃣ **Mapping Type**
- **`dict`** – Key-value pairs (e.g., `{'name': 'Alice', 'age': 25}`)

### 6️⃣ **Boolean Type**
- **`bool`** – Represents `True` or `False`

### 7️⃣ **Binary Types**
- **`bytes`** – Immutable sequence of bytes
- **`bytearray`** – Mutable sequence of bytes
- **`memoryview`** – Memory-efficient view of binary data

## 🔎 Checking Data Types
Use the `type()` function to check the type of a variable:
```python
x = 10
print(type(x))  # Output: <class 'int'>
```

## 🔄 Type Conversion (Type Casting)
Convert one data type to another using built-in functions:
```python
x = 5  # int
y = float(x)  # Convert int to float
z = str(x)  # Convert int to string
```

## 🚀 Summary
| Category    | Data Types |
|------------|-----------|
| Numeric    | `int`, `float`, `complex` |
| Text       | `str` |
| Sequence   | `list`, `tuple`, `range` |
| Set        | `set`, `frozenset` |
| Mapping    | `dict` |
| Boolean    | `bool` |
| Binary     | `bytes`, `bytearray`, `memoryview` |

Understanding these data types is crucial for working with Python efficiently. Happy Coding! 🚀


#### More Examples:
```python
print("Python is awesome!")
print(5 + 3)
print("The sum of 5 and 3 is", 5 + 3)
print("Python", "is", "fun", sep="-")
print("Python", end="!")
print("Learning Python")
print("\nThis is a new line character example.")
print("\tThis is a tab space example.")
print(r"This is a raw string: \n will not create a new line")
print("Multiline\nstring\nexample")
```

---

##  Variables and Data Types
### Topics Covered:
- Understanding variables and data types
- Strings, integers, floats, and Boolean values
- Type conversion and type checking
- Input and output functions

### Theory:
Variables store data that can be used and manipulated in a program. Python supports dynamic typing, meaning you don’t need to declare variable types explicitly.

### Hands-on Practice:
```python
# Declaring variables
name = "Alice"
age = 25
height = 5.6
is_student = True

# Printing variables
print(name, age, height, is_student)

# Taking user input
user_name = input("Enter your name: ")
print("Hello,", user_name)
```

#### More Examples:
```python
x = 10
print(type(x))
y = 3.14
print(type(y))
z = "Python"
print(type(z))
a = True
print(type(a))
b = int("123")
print(b)
c = float("12.34")
print(c)
d = str(100)
print(d)
e = bool(1)
print(e)
f = bool(0)
print(f)
```

---

## Class 3: Control Flow - Conditional Statements
### Topics Covered:
- If, elif, and else statements
- Logical and comparison operators
- Nested conditions and best practices

### Theory:
Conditional statements allow the program to make decisions based on conditions. The `if` statement executes a block of code if the condition is true.

### Hands-on Practice:
```python
num = int(input("Enter a number: "))
if num % 2 == 0:
    print("Even number")
else:
    print("Odd number")
```

#### More Examples:
```python
x = 10
y = 20
if x > y:
    print("x is greater than y")
elif x < y:
    print("x is less than y")
else:
    print("x is equal to y")

age = int(input("Enter your age: "))
if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")

score = 85
if score >= 90:
    print("Grade A")
elif score >= 80:
    print("Grade B")
elif score >= 70:
    print("Grade C")
else:
    print("Grade D")
```

---

## Class 4: Loops and Iteration
### Topics Covered:
- For and while loops
- Loop control statements (`break`, `continue`, `pass`)
- Iterating through lists and strings

### Theory:
Loops allow executing a block of code multiple times. The `for` loop is used for iterating over sequences, while the `while` loop continues running as long as the condition is true.

### Hands-on Practice:
```python
# Using a for loop
for i in range(1, 11):
    print(i)

# Using a while loop
count = 1
while count <= 5:
    print("Iteration", count)
    count += 1
```

#### More Examples:
```python
for i in "Python":
    print(i)

nums = [10, 20, 30, 40]
for num in nums:
    print(num)

x = 0
while x < 5:
    print(x)
    x += 1

for i in range(10):
    if i == 5:
        break
    print(i)
```

---

## Class 5: Functions and Modules
### Topics Covered:
- Defining and calling functions
- Function parameters and return values
- Using built-in functions
- Importing and using modules

### Theory:
Functions help in organizing code into reusable blocks. Python also allows importing modules to extend functionality.

### Hands-on Practice:
```python
# Defining a function
def greet(name):
    return f"Hello, {name}!"

# Calling the function
print(greet("Alice"))

# Using the math module
import math
print("Square root of 16:", math.sqrt(16))
```

#### More Examples:
```python
def add(a, b):
    return a + b

print(add(5, 3))

def is_even(n):
    return n % 2 == 0

print(is_even(10))
print(is_even(7))

def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n - 1)

print(factorial(5))
```

---

## Next Steps
- Exploring data structures (lists, tuples, dictionaries)
- Understanding file handling
- Introduction to object-oriented programming
- Practical projects and real-world applications
