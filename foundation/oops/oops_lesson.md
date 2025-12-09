# OOPs Full Lesson for Beginners

## 1. What is OOP?

Object-Oriented Programming (OOP) is a style of programming...

## 2. Why OOP?

-   Modular code
-   Reduced repetition
-   Easy to maintain
-   Secure

## 3. Key Concepts

1.  Class\
2.  Object\
3.  Encapsulation\
4.  Abstraction\
5.  Inheritance\
6.  Polymorphism\
7.  Constructor & Destructor\
8.  Method Overloading\
9.  Method Overriding\
10. Composition

## 4. Class

**Theory:** A class is a blueprint...

``` python
class Car:
    brand = "BMW"
    color = "Black"

    def show(self):
        print("Brand:", self.brand, "Color:", self.color)
```

## 5. Object

**Theory:** Object is an instance...

``` python
class Car:
    def __init__(self, brand, color):
        self.brand = brand
        self.color = color
```

## 6. Encapsulation

**Theory:** Protects data...

``` python
class Bank:
    def __init__(self):
        self.__balance = 1000
```

## 7. Abstraction

**Theory:** Hides complexity...

``` python
from abc import ABC, abstractmethod
```

## 8. Inheritance

**Theory:** Reuse parent class...

``` python
class Animal:
    def eat(self):
        print("Eating")
```

## 9. Polymorphism

**Theory:** Same method, different behavior...

``` python
class Dog:
    def sound(self):
        print("Bark")
```

## 10. Constructor & Destructor

``` python
def __init__(self):
    pass
```

## 11. Overloading & Overriding

``` python
def add(self, a, b, c=0):
    return a + b + c
```

## 12. Composition

``` python
class Engine:
    pass
```
