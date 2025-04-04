
# Python Data Structures: Tuple, Set, and Dictionary
If a data type supports indexing, it is ordered. Ex - list , dictionary , tuple , string are ordered and set is not ordered 
### Examples of Ordered (Indexable) Types

| Data Type | Ordered? | Indexing?        |
|-----------|----------|------------------|
| `list`    | ✅ Yes   | ✅ Yes (by index) |
| `tuple`   | ✅ Yes   | ✅ Yes (by index) |
| `str`     | ✅ Yes   | ✅ Yes (by index) |
| `dict` (since Python 3.7+) | ✅ Yes (insertion order) | ✅ Yes (by key only) |


## 1. Tuple
A **tuple** is an immutable, ordered collection of elements.

### Creating a Tuple
```python
# Creating a tuple
tuple1 = (1, 2, 3, 4, 5)
tuple2 = ('apple', 'banana', 'cherry')
```

### Accessing Elements
```python
print(tuple1[0])  # Output: 1
print(tuple2[-1])  # Output: 'cherry'
```

### Tuple Methods
```python
print(len(tuple1))  # Output: 5
print(tuple1.count(2))  # Output: 1
print(tuple1.index(3))  # Output: 2
```

---

## 2. Set
A **set** is an unordered collection of unique elements.

Unordered: It does not maintain any specific order of elements. indexing and slicing possible 

Unique: It automatically removes duplicates — each element appears only once

my_set = {'apple', 'banana', 'cherry', 'apple'}

print(my_set)

output= {'banana', 'cherry', 'apple'}


### Creating a Set
```python
set1 = {1, 2, 3, 4, 5}
set2 = set(["apple", "banana", "cherry"])
```

### Adding and Removing Elements
```python
set1.add(6)  # Adds 6 to the set
set1.remove(3)  # Removes 3 from the set
```

### Set Operations
```python
setA = {1, 2, 3, 4}
setB = {3, 4, 5, 6}
print(setA.union(setB))  # {1, 2, 3, 4, 5, 6}
print(setA.intersection(setB))  # {3, 4}
print(setA.difference(setB))  # {1, 2}
```

---

## 3. Dictionary
A **dictionary** is a collection of key-value pairs.

### Creating a Dictionary
```python
dict1 = {
    "name": "Alice",
    "age": 25,
    "city": "New York"
}
```

### Accessing Elements
```python
print(dict1["name"])  # Output: Alice
print(dict1.get("age"))  # Output: 25
```

### Adding and Removing Elements
```python
dict1["country"] = "USA"  # Adds a new key-value pair
del dict1["city"]  # Removes key 'city'
```

### Dictionary Methods
```python
print(dict1.keys())  # Returns all keys
print(dict1.values())  # Returns all values
print(dict1.items())  # Returns all key-value pairs
```

---
### Comparison of List, Tuple, Set, and Dictionary

| Feature       | List  | Tuple | Set  | Dictionary |
|--------------|-------|-------|------|------------|
| Ordered      | ✅ Yes | ✅ Yes | ❌ No | ✅ Yes (from Python 3.7+) |
| Mutable      | ✅ Yes | ❌ No | ✅ Yes | ✅ Yes |
| Allows Duplicates | ✅ Yes | ✅ Yes | ❌ No | ❌ No (Keys) |
| Indexed Access | ✅ Yes | ✅ Yes | ❌ No | ✅ Yes (Keys) |
| Iteration    | ✅ Yes | ✅ Yes | ✅ Yes | ✅ Yes |
| Key-Value Structure | ❌ No | ❌ No | ❌ No | ✅ Yes |

This guide provides an overview of **lists, tuples, sets, and dictionaries** in Python, highlighting their properties, operations, and common methods.
