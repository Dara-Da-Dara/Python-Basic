# Lists in Python

A **list** is a built-in **mutable** data type in Python that allows storing multiple values in an ordered sequence.

## **1. Creating a List**
Lists are created using square brackets `[]`.

```python
# Creating a list with different data types
my_list = [1, 2, 3, "Python", 4.5]
print(my_list)  # Output: [1, 2, 3, 'Python', 4.5]

2. Accessing Elements
You can access list elements using indexing and slicing.

Indexing
my_list = [10, 20, 30, 40]
print(my_list[0])   # Output: 10
print(my_list[-1])  # Output: 40 (Last element)

Slicing
my_list = [1, 2, 3, 4, 5, 6]
print(my_list[1:4])  # Output: [2, 3, 4]

3. Modifying a List (Mutable)
Lists are mutable, meaning you can change, add, or remove elements.

my_list = [10, 20, 30]
my_list[1] = 50
print(my_list)  # Output: [10, 50, 30]

Adding Elements

my_list.append(40)  # Adds at the end
print(my_list)  # Output: [10, 50, 30, 40]

my_list.insert(1, 25)  # Inserts at index 1
print(my_list)  # Output: [10, 25, 50, 30, 40]
Removing Elements

my_list.remove(50)  # Removes first occurrence of 50
print(my_list)  # Output: [10, 25, 30, 40]

popped_element = my_list.pop()  # Removes last element
print(popped_element)  # Output: 40
print(my_list)  # Output: [10, 25, 30]

4. Looping Through a List
You can iterate through a list using a loop.

Using a for loop
python
Copy
Edit
my_list = ["Apple", "Banana", "Cherry"]
for fruit in my_list:
    print(fruit)
# Output:
# Apple
# Banana
# Cherry

Using enumerate()

for index, value in enumerate(my_list):
    print(index, value)
# Output:
# 0 Apple
# 1 Banana
# 2 Cherry
5. List Comprehension
A concise way to create lists.


squares = [x**2 for x in range(1, 6)]
print(squares)  # Output: [1, 4, 9, 16, 25]

6. Common List Methods

Method	Description	Example
append(x)	Adds x to the end of the list.	my_list.append(10)
insert(i, x)	Inserts x at index i.	my_list.insert(1, 20)
remove(x)	Removes first occurrence of x.	my_list.remove(10)
pop(i)	Removes and returns the element at index i (default: last).	my_list.pop(2)
sort()	Sorts the list in ascending order.	my_list.sort()
reverse()	Reverses the list.	my_list.reverse()
index(x)	Returns the index of first occurrence of x.	my_list.index(30)
count(x)	Returns the count of occurrences of x.	my_list.count(10)
7. List vs. Tuple
Feature	List (list)	Tuple (tuple)
Mutable?	✅ Yes	❌ No
Ordered?	✅ Yes	✅ Yes
Performance	❌ Slower	✅ Faster
Uses	✅ Dynamic, frequently changing data	✅ Fixed, constant data

8. Nested Lists
Lists can contain other lists, creating a nested structure.


nested_list = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
print(nested_list[1])   # Output: [4, 5, 6]
print(nested_list[1][2])  # Output: 6
9. List Copying
Copying a list requires caution to avoid unintended modifications.

Shallow Copy (Reference Copy)
python
Copy
Edit
list1 = [1, 2, 3]
list2 = list1  # Both lists point to the same memory location
list2.append(4)
print(list1)  # Output: [1, 2, 3, 4] (Also modified)
Deep Copy (Independent Copy)

import copy
list1 = [1, 2, 3]
list2 = copy.deepcopy(list1)  # Creates an independent copy
list2.append(4)
print(list1)  # Output: [1, 2, 3] (Unchanged)
10. Sorting a List
Lists can be sorted in ascending or descending order.


numbers = [4, 1, 3, 5, 2]
numbers.sort()  # Sorts in ascending order
print(numbers)  # Output: [1, 2, 3, 4, 5]

numbers.sort(reverse=True)  # Sorts in descending order
print(numbers)  # Output: [5, 4, 3, 2, 1]
11. List Operations
Concatenation

list1 = [1, 2, 3]
list2 = [4, 5, 6]
combined_list = list1 + list2
print(combined_list)  # Output: [1, 2, 3, 4, 5, 6]
Repetition

my_list = [1, 2, 3]
print(my_list * 3)  # Output: [1, 2, 3, 1, 2, 3, 1, 2, 3]
Membership Check
python
Copy
Edit
my_list = [10, 20, 30]
print(20 in my_list)  # Output: True
print(50 in my_list)  # Output: False
12. List Memory Efficiency
Since lists are dynamic, they use more memory than tuples.


import sys
list_obj = [1, 2, 3, 4, 5]
tuple_obj = (1, 2, 3, 4, 5)

print(sys.getsizeof(list_obj))  # Output: (larger size)
print(sys.getsizeof(tuple_obj)) # Output: (smaller size)
Conclusion
Lists are ordered, mutable, and allow duplicate values.

You can modify, add, or remove elements easily.

List comprehension helps in efficient list creation.

Use lists for dynamic data, while tuples are better for fixed data.










