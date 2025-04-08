
# 🔢 NumPy Full Class - Numerical Python Library

Welcome to the **NumPy Full Class**! This guide covers everything from installation to advanced numerical computing using **NumPy** in Python.

---

## 📦 Installation

```bash
pip install numpy
```

---

## 📘 Importing NumPy

```python
import numpy as np
```

---

## 📊 Creating Arrays

### 1D Array

```python
a = np.array([1, 2, 3])
print(a)
```

### 2D Array

```python
b = np.array([[1, 2], [3, 4]])
print(b)
```

### 3D Array

```python
c = np.array([[[1], [2]], [[3], [4]]])
print(c)
```

---

## 🛠️ Array Attributes

```python
a.shape       # Shape of array
a.ndim        # Number of dimensions
a.size        # Number of elements
a.dtype       # Data type of elements
```

---

## 📏 Array Creation Methods

```python
np.zeros((2, 3))           # Array of zeros
np.ones((2, 3))            # Array of ones
np.full((2, 2), 7)         # Array filled with a constant
np.eye(3)                  # Identity matrix
np.arange(0, 10, 2)        # Evenly spaced values
np.linspace(0, 1, 5)       # 5 numbers from 0 to 1
```

---

## 🔄 Reshaping & Resizing

```python
a = np.arange(6)          # [0, 1, 2, 3, 4, 5]
a.reshape((2, 3))         # Reshape to 2x3
a.resize((3, 2))          # Resize to 3x2
```

---

## 🔍 Indexing & Slicing

```python
a = np.array([1, 2, 3, 4])
a[1]                      # Access element at index 1
a[1:3]                    # Slice from index 1 to 2
a[-1]                     # Last element
```

---

## ➕ Mathematical Operations

```python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])

a + b                     # Element-wise addition
a - b                     # Subtraction
a * b                     # Multiplication
a / b                     # Division
np.dot(a, b)              # Dot product
```

---

## 🧠 Useful Functions

```python
np.mean(a)                # Mean
np.median(a)              # Median
np.std(a)                 # Standard deviation
np.max(a)                 # Max value
np.min(a)                 # Min value
np.sum(a)                 # Sum
np.unique(a)              # Unique values
```

---

## 🔀 Random Numbers

```python
np.random.rand(2, 3)      # Random floats in [0, 1)
np.random.randint(0, 10, size=(3, 3))  # Random integers
```

---

## 🎯 Boolean Masking & Filtering

```python
a = np.array([1, 2, 3, 4])
mask = a > 2              # [False, False, True, True]
a[mask]                   # [3, 4]
```

---

## ♻️ Broadcasting

```python
a = np.array([1, 2, 3])
b = 2
a + b                     # [3, 4, 5]
```

---

## 🧹 Handling NaN

```python
a = np.array([1, np.nan, 3])
np.isnan(a)               # [False, True, False]
np.nanmean(a)             # Mean ignoring NaN
```

---

## 📚 References

- [NumPy Official Docs](https://numpy.org/doc/)
- [NumPy GitHub](https://github.com/numpy/numpy)

---

## 🏁 Final Example

```python
import numpy as np

matrix = np.random.randint(1, 10, size=(3, 3))
print("Matrix:")
print(matrix)

inv = np.linalg.inv(matrix)
print("Inverse:")
print(inv)
```

---

## 🙌 Happy Learning NumPy!
