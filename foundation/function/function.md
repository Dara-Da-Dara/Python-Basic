# **Python Functions **  

## **1. Introduction to Functions**  
A function in Python is a reusable block of code that performs a specific task. Functions help in organizing and structuring code efficiently.  

### **Why Use Functions?**  
- **Code Reusability** – Write once, use multiple times.  
- **Improves Readability** – Breaks complex problems into smaller, manageable parts.  
- **Reduces Redundancy** – Avoids repetition of the same code.  
- **Easier Debugging** – Errors are isolated within functions.  

---

## **2. Defining and Calling a Function**  

### **Defining a Function**  
In Python, a function is defined using the `def` keyword.  

#### **Syntax**  
```python
 def function_name(parameters):
     """Optional docstring"""
     # Function body
     return value  # Optional
```  

#### **Example: Simple Function Without Parameters**  
```python
 def greet():
     print("Hello, Students!")

 greet()  # Calling the function
```
**Output:**  
```
 Hello, Students!
```

#### **Example: Function With Parameters**  
```python
 def greet(name):
     print("Hello,", name)

 greet("John")
```
**Output:**  
```
 Hello, John
```
### 
| With `return`               | Without `return`                         |
| --------------------------- | ---------------------------------------- |
| Function sends a value back | Function does an action only             |
| Can store in a variable     | Nothing returned (Python returns `None`) |
| Useful for calculations     | Useful for printing or updating things   |

---

## **3. Function Parameters and Arguments**  
Functions can take inputs, known as parameters, to process data.  

### **Types of Arguments in Python Functions**  
1. **Positional Arguments**  
2. **Keyword Arguments**  
3. **Default Arguments**  
4. **Arbitrary Arguments (`*args` and `**kwargs`)**  

### **1. Positional Arguments**  
Arguments are passed in the same order as the function definition.  

```python
 def student_details(name, age):
     print("Name:", name)
     print("Age:", age)

 student_details("Alice", 20)
```
**Output:**  
```
 Name: Alice  
 Age: 20  
```

### **2. Keyword Arguments**  
Arguments are passed using the parameter name explicitly.  

```python
 student_details(age=22, name="Bob")
```
**Output:**  
```
 Name: Bob  
 Age: 22  
```

### **3. Default Arguments**  
If an argument is not provided, it takes a default value.  

```python
 def greet(name="Student"):
     print("Hello,", name)

 greet()  
 greet("David")
```
**Output:**  
```
 Hello, Student  
 Hello, David  
```

### **4. Arbitrary Arguments (`*args` and `**kwargs`)**  
#### **Using `*args` for Multiple Positional Arguments**  
```python
 def add_numbers(*numbers):
     total = sum(numbers)
     print("Sum:", total)

 add_numbers(10, 20, 30, 40)
```
**Output:**  
```
 Sum: 100
```

#### **Using `**kwargs` for Multiple Keyword Arguments**  
```python
 def student_info(**details):
     for key, value in details.items():
         print(key, ":", value)

 student_info(name="Emma", age=21, course="AI")
```
**Output:**  
```
 name : Emma  
 age : 21  
 course : AI  
```

---

## **4. Return Statement**  
Functions can return values using the `return` keyword.  

```python
 def square(num):
     return num * num

 result = square(5)
 print("Square:", result)
```
**Output:**  
```
 Square: 25
```

---

## **5. Lambda Functions (Anonymous Functions)**  
A lambda function is a small, anonymous function defined using the `lambda` keyword.  

```python
 square = lambda x: x * x
 print(square(5))
```
**Output:**  
```
 25
```

```python
 add = lambda a, b: a + b
 print(add(3, 7))
```
**Output:**  
```
 10
```

---

## **6. Scope and Lifetime of Variables**  
### **1. Local Scope**  
Variables declared inside a function are local to that function.  

```python
 def func():
     x = 10  # Local variable
     print(x)

 func()
```

### **2. Global Scope**  
A variable declared outside a function is accessible anywhere in the program.  

```python
 x = 20  # Global variable

def func():
     print(x)

 func()
```
**Output:**  
```
 20
```

---

## **7. Nested Functions**  
A function inside another function.  

```python
 def outer():
     def inner():
         print("This is inner function")
     inner()

 outer()
```
**Output:**  
```
 This is inner function
```

---

## **8. Recursive Functions**  
A function that calls itself to solve a problem.  

### **Example: Factorial Calculation**  
```python
 def factorial(n):
     if n == 0:
         return 1
     else:
         return n * factorial(n - 1)

 print(factorial(5))
```
**Output:**  
```
 120
```

---

## **9. Function as an Argument**  
Functions can be passed as arguments to other functions.  

```python
 def greet(name):
     return "Hello " + name

def call_func(func, name):
     print(func(name))

 call_func(greet, "Alice")
```
**Output:**  
```
 Hello Alice
```

---

## **10. Built-in Functions in Python**  
Python has several built-in functions, including:  

- `print()`
- `len()`
- `type()`
- `abs()`
- `sum()`
- `max()`
- `min()`
- `sorted()`
- `map()`
- `filter()`
- `zip()`

---


## **Key Takeaways**  
- Functions help in code reusability and organization.  
- Python supports different types of function arguments (`positional`, `keyword`, `default`, `*args`, `**kwargs`).  
- Functions can return values using the `return` keyword.  
- `lambda` functions allow quick, one-line function definitions.  
- Scope defines where a variable can be accessed (`local`, `global`).  
- Recursive functions call themselves to solve problems like factorial and Fibonacci series.  
- Functions can be passed as arguments and returned as values.  
- Python provides built-in functions for common operations.  

This chapter provides a strong foundation for mastering Python functions. 🚀
