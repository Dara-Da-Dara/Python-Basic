
# 🌀 Python `for` Loop - A Beginner's Guide

## 📘 What is a `for` loop?

A `for` loop in Python is used to iterate over a sequence (like a list, tuple, dictionary, set, or string). 
This allows you to execute a block of code multiple times.

---

## 🔁 Syntax

```python
for variable in sequence:
    # code block to execute
```

---

## 🧪 Examples

### 1. Looping through a list

```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```

🖨️ Output:
```
apple
banana
cherry
```

---

### 2. Looping through a string

```python
for char in "hello":
    print(char)
```

🖨️ Output:
```
h
e
l
l
o
```

---

### 3. Using `range()`

```python
for i in range(5):
    print(i)
```

🖨️ Output:
```
0
1
2
3
4
```

---

### 4. Using `else` with `for` loop

```python
for i in range(3):
    print(i)
else:
    print("Loop finished!")
```

🖨️ Output:
```
0
1
2
Loop finished!
```

---

## ⛔ Using `break` to exit the loop

```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

🖨️ Output:
```
0
1
2
3
4
```

---

## ↪️ Using `continue` to skip an iteration

```python
for i in range(6):
    if i == 3:
        continue
    print(i)
```

🖨️ Output:
```
0
1
2
4
5
```

---

## 📚 Looping through a dictionary

```python
student_scores = {"Alice": 85, "Bob": 92, "Charlie": 78}
for student, score in student_scores.items():
    print(f"{student} scored {score}")
```

🖨️ Output:
```
Alice scored 85
Bob scored 92
Charlie scored 78
```

---

## 💡 Tips

- Use `enumerate()` to get both index and value:
  
```python
colors = ["red", "green", "blue"]
for index, color in enumerate(colors):
    print(index, color)
```

- Use `zip()` to iterate over multiple sequences together:

```python
names = ["Tom", "Jerry", "Spike"]
scores = [80, 90, 70]
for name, score in zip(names, scores):
    print(f"{name}: {score}")
```

---

## 🧩 Practice Exercises

### Exercise 1
Write a `for` loop that prints all even numbers from 1 to 20.

### Exercise 2
Create a list of numbers from 1 to 10. Print the square of each number using a `for` loop.

### Exercise 3
Loop through a string and count how many vowels it contains.

<details>
<summary>Hint 🔍</summary>

Use `if` conditions and a counter variable.

</details>

---

## ✅ Summary

- `for` loops are used for iterating over sequences.
- Can be combined with `range()`, `break`, `continue`, `enumerate()`, and `zip()`.
- Useful for repetitive tasks like printing, calculations, or data processing.

---

## 📂 Save and Share

Fork this repo and add your own examples to expand your understanding.
Happy coding! 🚀
