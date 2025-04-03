# Lists in Python

A **list** is a built-in **mutable** data type in Python that allows storing multiple values in an ordered sequence.

## **1. Creating a List**
Lists are created using square brackets `[]`.

```python
# Creating a list with different data types
my_list = [1, 2, 3, "Python", 4.5]
print(my_list)  # Output: [1, 2, 3, 'Python', 4.5]
```

## **2. Accessing Elements**
You can access list elements using indexing and slicing.

### **Indexing**
```python
my_list = [10, 20, 30, 40]
print(my_list[0])   # Output: 10
print(my_list[-1])  # Output: 40 (Last element)
```

### **Slicing**
```python
my_list = [1, 2, 3, 4, 5, 6]
print(my_list[1:4])  # Output: [2, 3, 4]
```

## **3. Modifying a List (Mutable)**
Lists are mutable, meaning you can change, add, or remove elements.

```python
my_list = [10, 20, 30]
my_list[1] = 50
print(my_list)  # Output: [10, 50, 30]
```

### **Adding Elements**
```python
my_list.append(40)  # Adds at the end
print(my_list)  # Output: [10, 50, 30, 40]

my_list.insert(1, 25)  # Inserts at index 1
print(my_list)  # Output: [10, 25, 50, 30, 40]
```

### **Removing Elements**
```python
my_list.remove(50)  # Removes first occurrence of 50
print(my_list)  # Output: [10, 25, 30, 40]

popped_element = my_list.pop()  # Removes last element
print(popped_element)  # Output: 40
print(my_list)  # Output: [10, 25, 30]
```

## **4. Looping Through a List**
You can iterate through a list using a loop.

### **Using a for loop**
```python
my_list = ["Apple", "Banana", "Cherry"]
for fruit in my_list:
    print(fruit)
```
#### **Output:**
```
Apple
Banana
Cherry
```

### **Using enumerate()**
```python
for index, value in enumerate(my_list):
    print(index, value)
```
#### **Output:**
```
0 Apple
1 Banana
2 Cherry
```

## **5. List Comprehension**
A concise way to create lists.

```python
squares = [x**2 for x in range(1, 6)]
print(squares)  # Output: [1, 4, 9, 16, 25]
```

## **6. Common List Methods**

| Method         | Description                                 | Example |
|---------------|---------------------------------------------|---------|
| `append(x)`   | Adds `x` to the end of the list.           | `my_list.append(10)` |
| `insert(i, x)`| Inserts `x` at index `i`.                  | `my_list.insert(1, 20)` |
| `remove(x)`   | Removes the first occurrence of `x`.       | `my_list.remove(10)` |
| `pop(i)`      | Removes and returns the element at index `i` (default: last). | `my_list.pop(2)` |
| `sort()`      | Sorts the list in ascending order.         | `my_list.sort()` |
| `reverse()`   | Reverses the list.                         | `my_list.reverse()` |
| `index(x)`    | Returns the index of the first occurrence of `x`. | `my_list.index(30)` |
| `count(x)`    | Returns the count of occurrences of `x`.   | `my_list.count(10)` |
| `copy()`      | Returns a shallow copy of the list.        | `new_list = my_list.copy()` |
| `extend(iterable)` | Extends the list by appending elements from another iterable. | `my_list.extend([5, 6, 7])` |
| `clear()`     | Removes all elements from the list.        | `my_list.clear()` |

## **7. List vs. Tuple**

| Feature       | List (`list`) | Tuple (`tuple`) |
|--------------|--------------|----------------|
| **Mutability** | ✅ Mutable (Can be changed) | ❌ Immutable (Cannot be changed) |
| **Ordering**   | ✅ Ordered  | ✅ Ordered  |
| **Performance** | ❌ Slower (due to dynamic resizing) | ✅ Faster (fixed size) |
| **Memory Usage** | ❌ Higher | ✅ Lower |
| **Use Case** | ✅ Suitable for frequently changing data | ✅ Suitable for fixed, constant data |
| **Methods Available** | ✅ More built-in methods like `append()`, `remove()` | ❌ Fewer built-in methods |
| **Iteration Speed** | ❌ Slower (due to dynamic resizing) | ✅ Faster |

## **8. Nested Lists**
Lists can contain other lists, creating a nested structure.

```python
nested_list = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
print(nested_list[1])   # Output: [4, 5, 6]
print(nested_list[1][2])  # Output: 6
```

## **9. List Copying**
Copying a list requires caution to avoid unintended modifications.

### **Shallow Copy (Reference Copy)**
```python
list1 = [1, 2, 3]
list2 = list1  # Both lists point to the same memory location
list2.append(4)
print(list1)  # Output: [1, 2, 3, 4] (Also modified)
```

### **Deep Copy (Independent Copy)**
```python
import copy
list1 = [1, 2, 3]
list2 = copy.deepcopy(list1)  # Creates an independent copy
list2.append(4)
print(list1)  # Output: [1, 2, 3] (Unchanged)
```

## **10. Sorting a List**
```python
numbers = [4, 1, 3, 5, 2]
numbers.sort()
print(numbers)  # Output: [1, 2, 3, 4, 5]
```

## **11. List Operations**
### **Concatenation**
```python
list1 = [1, 2, 3]
list2 = [4, 5, 6]
combined_list = list1 + list2
print(combined_list)  # Output: [1, 2, 3, 4, 5, 6]
```

### **Membership Check**
```python
my_list = [10, 20, 30]
print(20 in my_list)  # Output: True
```

## **Conclusion**
- Lists are ordered, mutable, and allow duplicate values.
- List comprehension helps in efficient list creation.
- Use lists for dynamic data, while tuples are better for fixed data.

