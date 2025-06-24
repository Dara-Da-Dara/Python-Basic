# 📘 NumPy Lesson: Comprehensive Guide

## 🧠 What is NumPy?

NumPy (Numerical Python) is a powerful library for numerical computing in Python. It provides:

- Efficient array storage and computation
- Functions for performing mathematical operations
- Tools for working with large datasets, matrices, and high-dimensional data

---

## 🔧 Installation

To install NumPy, use:

```bash
pip install numpy
```

---

## 📦 Importing NumPy

Conventionally, NumPy is imported as `np`:

```python
import numpy as np
```

---

## 🔢 NumPy Arrays

### Creating Arrays

```python
a = np.array([1, 2, 3])
b = np.array([[1, 2], [3, 4]])
```

### Array Attributes

- `ndim`: Number of dimensions
- `shape`: Shape of the array
- `size`: Total number of elements
- `dtype`: Data type of the elements

```python
print(b.ndim)  # 2
print(b.shape)  # (2, 2)
print(b.size)   # 4
```

---

## 🏗️ Array Creation Functions

- `np.zeros(shape)` → Array of zeros
- `np.ones(shape)` → Array of ones
- `np.full(shape, fill_value)` → Array filled with a specific value
- `np.eye(n)` → Identity matrix
- `np.arange(start, stop, step)` → Array with a range of values
- `np.linspace(start, stop, num)` → Evenly spaced numbers over interval

```python
np.zeros((2, 3))
np.eye(3)
```

---

## 🧮 Array Operations

### Element-wise Arithmetic

```python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])

print(a + b)
print(a * b)
print(a / b)
```

### Matrix Multiplication

```python
A = np.array([[1, 2], [3, 4]])
B = np.array([[2, 0], [1, 3]])

C = A @ B  # or np.dot(A, B)
```

---

## 🔁 Indexing and Slicing

```python
a = np.array([[1, 2, 3], [4, 5, 6]])
print(a[1, 2])   # 6
print(a[:, 1])   # [2 5]
```

### Boolean Indexing

```python
a = np.array([1, 2, 3, 4])
print(a[a > 2])  # [3 4]
```

### Fancy Indexing

```python
a = np.array([10, 20, 30, 40, 50])
indices = [1, 3]
print(a[indices])  # [20 40]
```

---

## 🔄 Array Manipulation

- `reshape()` – Change shape without changing data
- `flatten()` – Flatten array to 1D
- `transpose()` – Swap axes

```python
a = np.array([[1, 2], [3, 4]])
a.reshape(4)
a.flatten()
a.T
```

---

## 📈 Aggregate Functions

- `np.sum()`, `np.mean()`, `np.std()`, `np.var()`
- `np.min()`, `np.max()`, `np.argmin()`, `np.argmax()`

```python
a = np.array([[1, 2], [3, 4]])
np.sum(a)
np.mean(a, axis=0)
```

---

## 🎲 Random Numbers

- `np.random.rand(d0, d1, ...)` → Uniform distribution
- `np.random.randn(d0, d1, ...)` → Standard normal distribution
- `np.random.randint(low, high, size)` → Random integers

```python
np.random.rand(2, 2)
np.random.randint(0, 10, size=(2, 3))
```

---

## ⚙️ Linear Algebra

- `np.linalg.inv()` – Inverse of a matrix
- `np.linalg.det()` – Determinant
- `np.linalg.eig()` – Eigenvalues and eigenvectors
- `np.linalg.solve()` – Solves linear matrix equations

```python
A = np.array([[1, 2], [3, 4]])
np.linalg.inv(A)
```

---

## 🧾 Summary

- NumPy is the foundation of numerical computing in Python.
- Arrays enable efficient vectorized operations.
- Use NumPy for large-scale data processing, machine learning, and scientific computing.

---

## 📚 Further Resources

- [NumPy User Guide](https://numpy.org/doc/stable/user/index.html)
- [NumPy Quickstart](https://numpy.org/doc/stable/user/quickstart.html)