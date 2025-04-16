# 🧠 Python Lesson: `if`, `else`, and `elif`

## ✅ What is an `if` statement?

An `if` statement is used to **make decisions** in Python. It allows you to execute certain blocks of code **only when a condition is true**.

---

## 🔹 Basic Syntax

```python
if condition:
    # code to run if condition is True
```

> **Note:** Python relies on **indentation** to define blocks of code.

---

## 🔹 Example 1: Simple `if`

```python
x = 10

if x > 5:
    print("x is greater than 5")
```

**Output:**
```
x is greater than 5
```

---

## 🔹 Adding `else`

The `else` block runs when the `if` condition is not true.

```python
x = 3

if x > 5:
    print("x is greater than 5")
else:
    print("x is 5 or less")
```

**Output:**
```
x is 5 or less
```

---

## 🔹 Using `elif` (short for "else if")

Use `elif` to test multiple conditions in order.

```python
x = 5

if x > 5:
    print("x is greater than 5")
elif x == 5:
    print("x is equal to 5")
else:
    print("x is less than 5")
```

**Output:**
```
x is equal to 5
```

---

## 🛠️ Practice Examples

### Example 1: Check if a number is positive or negative

```python
num = -2

if num > 0:
    print("Positive number")
else:
    print("Negative number")
```

---

### Example 2: Even or Odd Checker

```python
num = 7

if num % 2 == 0:
    print("Even number")
else:
    print("Odd number")
```

---

## 🧪 Try it Yourself

- Write a program to check whether a number is divisible by 3 and 5.
- Create a grading system using `if`, `elif`, and `else`:
    - 90 and above: A
    - 80-89: B
    - 70-79: C
    - Below 70: F
