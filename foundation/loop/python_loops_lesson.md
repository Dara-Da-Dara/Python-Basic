
#  Python Loops Lesson

## 📌 Introduction to Loops
Loops are used to **execute a block of code repeatedly**. Python has two main types of loops:
- `for` loop
- `while` loop

---

## 🔁 `for` Loop

The `for` loop is used to iterate over a **sequence** (like a list, tuple, dictionary, string, or range).

### ✅ Syntax:
```python
for variable in sequence:
    # code block
```

### 🔍 Example: Loop through a list
```python
fruits = ['apple', 'banana', 'cherry']
for fruit in fruits:
    print(fruit)
```

### 🔍 Example: Using `range()`
```python
for i in range(5):
    print(i)
```
> `range(5)` gives: 0, 1, 2, 3, 4

---

## 🔁 `while` Loop

The `while` loop runs **as long as a condition is true**.

### ✅ Syntax:
```python
while condition:
    # code block
```

### 🔍 Example:
```python
count = 0
while count < 5:
    print(count)
    count += 1
```

---

## 🛑 Loop Control Statements

### 🔹 `break`
Stops the loop immediately.
```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

### 🔹 `continue`
Skips the current iteration and moves to the next.
```python
for i in range(5):
    if i == 2:
        continue
    print(i)
```

### 🔹 `else` with loop
Runs when loop completes normally (no `break`).
```python
for i in range(3):
    print(i)
else:
    print("Done!")
```

---

## 🧠 Practice Exercise

1. Write a loop to print numbers from 1 to 10.
2. Write a `for` loop to print each character of your name.
3. Write a `while` loop that prints numbers until the number is divisible by 7.
