
# 📊 Python Lesson: Introduction to Matplotlib

`matplotlib` is a powerful library in Python for **data visualization**. It helps you create charts like line plots, bar graphs, scatter plots, and more.

---

## 📦 Installation

Install it using pip (if not already installed):

```bash
pip install matplotlib
```

---

## 📚 Importing the Library

```python
import matplotlib.pyplot as plt
```

---

## 📈 Line Plot

### 🔹 Basic Line Plot

```python
x = [1, 2, 3, 4, 5]
y = [10, 20, 25, 30, 40]

plt.plot(x, y)
plt.title("Line Plot Example")
plt.xlabel("X-axis")
plt.ylabel("Y-axis")
plt.show()
```

---

## 📊 Bar Chart

```python
categories = ['A', 'B', 'C', 'D']
values = [3, 7, 8, 5]

plt.bar(categories, values)
plt.title("Bar Chart Example")
plt.show()
```

---

## 🔵 Scatter Plot

```python
x = [5, 7, 8, 7, 2, 17]
y = [99, 86, 87, 88, 100, 86]

plt.scatter(x, y)
plt.title("Scatter Plot Example")
plt.xlabel("X-axis")
plt.ylabel("Y-axis")
plt.show()
```

---

## 📊 Pie Chart

```python
labels = ['Apples', 'Bananas', 'Cherries', 'Dates']
sizes = [15, 30, 45, 10]

plt.pie(sizes, labels=labels, autopct='%1.1f%%')
plt.title("Pie Chart Example")
plt.show()
```

---

## 🎨 Customization Tips

- `color='red'` → Change plot color
- `linestyle='--'` → Dashed line
- `marker='o'` → Add markers to data points

---

## 🧠 Practice Exercise

1. Create a line plot of your monthly expenses.
2. Make a bar chart showing sales of 4 products.
3. Draw a pie chart showing percentage of time spent on activities in a day.

---

Let me know if you'd like to see more examples or convert this to PDF!
