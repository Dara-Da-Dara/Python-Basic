
# 🧠 Complete Lesson on `while` Loops in Python

---

## 📘 1. What is a `while` Loop?

A `while` loop is used to execute a block of code repeatedly **as long as a condition remains `True`**.

---

## 🔤 2. Basic Syntax

```python
while condition:
    # Block of code to execute
```

### ➕ Explanation:
- `condition`: A boolean expression.
- If the condition is `True`, the block of code runs.
- Python checks the condition **before** each loop iteration.

---

## 🔁 3. Example: Counting from 1 to 5

```python
i = 1
while i <= 5:
    print(i)
    i += 1
```

### 📥 Output:
```
1
2
3
4
5
```

---

## 🚨 4. Infinite Loop

A loop that **never ends** because the condition is always true.

```python
# Be careful with infinite loops!
while True:
    print("This will print forever!")
```

🔐 **Tip**: Always make sure the condition will eventually become `False`!

---

## 🧯 5. Using `break` to Stop a Loop

The `break` statement stops the loop **immediately**.

```python
i = 1
while i <= 10:
    print(i)
    if i == 5:
        break  # exit the loop
    i += 1
```

### 🔚 Output:
```
1
2
3
4
5
```

---

## 🔄 6. Using `continue` to Skip an Iteration

The `continue` statement **skips** the current iteration and jumps to the next.

```python
i = 0
while i < 10:
    i += 1
    if i % 2 == 0:
        continue  # skip even numbers
    print(i)
```

### 📤 Output:
```
1
3
5
7
9
```

---

## 💬 7. While Loop with User Input

```python
password = ""
while password != "1234":
    password = input("Enter password: ")
print("Access granted!")
```

---

## 💡 8. Real-World Applications

- Repeating a menu until user exits
- Login systems
- Retry operations (e.g., network requests)
- Timers, animations in games

---

## 🎯 9. Nested `while` Loops

```python
i = 1
while i <= 3:
    j = 1
    while j <= 2:
        print(f"i = {i}, j = {j}")
        j += 1
    i += 1
```

---

## 🧪 10. Practice Exercises

### 🔸 Exercise 1:
Print numbers from 10 to 1 (reverse order).

### 🔸 Exercise 2:
Keep asking the user to guess a number until they get it right.

```python
correct_number = 7
guess = 0
while guess != correct_number:
    guess = int(input("Guess the number: "))
print("Correct!")
```

---

## 🧠 11. Challenge: Multiplication Table Generator

Ask the user for a number, then print its multiplication table up to 10 using a `while` loop.

```python
num = int(input("Enter a number: "))
i = 1
while i <= 10:
    print(f"{num} x {i} = {num * i}")
    i += 1
```

---

## ✅ Summary:

| Concept          | Description                          |
|------------------|--------------------------------------|
| `while`          | Repeats a block while condition is True |
| `break`          | Exits the loop early                 |
| `continue`       | Skips the current iteration          |
| Infinite loop    | Loop with a condition that never ends |
