
# Python `while` Loop Examples and Shorthand Operators

## 🔁 What is `!=`?
`!=` means **"not equal to"** in Python.

### Example:
```python
x = 5
if x != 3:
    print("x is not equal to 3")
```

**Output:**
```
x is not equal to 3
```

---

## 🔁 What is `*=`?
`*=` means **"multiply and assign"**. It's a shorthand for:
```python
x *= y  # same as x = x * y
```

### Example:
```python
x = 5
x *= 2
print(x)
```

**Output:**
```
10
```

---

## 🔁 40 Simple `while` Loop Examples in Python

### ✅ Basic Print & Number Examples

1. **Print numbers from 1 to 5**
```python
i = 1
while i <= 5:
    print(i)
    i += 1
```

2. **Print "Hello" 3 times**
```python
i = 0
while i < 3:
    print("Hello")
    i += 1
```

3. **Print even numbers from 2 to 10**
```python
i = 2
while i <= 10:
    print(i)
    i += 2
```

4. **Print odd numbers from 1 to 9**
```python
i = 1
while i < 10:
    print(i)
    i += 2
```

5. **Countdown from 5 to 1**
```python
i = 5
while i > 0:
    print(i)
    i -= 1
```

6. **Print squares of numbers from 1 to 5**
```python
i = 1
while i <= 5:
    print(i * i)
    i += 1
```

7. **Print table of 3**
```python
i = 1
while i <= 10:
    print(3 * i)
    i += 1
```

8. **Print numbers from 10 to 1**
```python
i = 10
while i >= 1:
    print(i)
    i -= 1
```

9. **Print "Python" 5 times**
```python
i = 0
while i < 5:
    print("Python")
    i += 1
```

10. **Sum numbers from 1 to 5**
```python
i = 1
sum = 0
while i <= 5:
    sum += i
    i += 1
print("Sum:", sum)
```

### ✅ User Input Examples

11. **Ask name until "stop" is entered**
```python
name = ""
while name != "stop":
    name = input("Enter name (type 'stop' to quit): ")
```

12. **Ask for correct password**
```python
pwd = ""
while pwd != "admin":
    pwd = input("Enter password: ")
```

13. **Input numbers until 0 is entered**
```python
num = 1
while num != 0:
    num = int(input("Enter number (0 to stop): "))
```

14. **Keep asking until correct answer is given**
```python
ans = ""
while ans != "blue":
    ans = input("What color is the sky? ")
```

15. **Ask age until age >= 18**
```python
age = 0
while age < 18:
    age = int(input("Enter your age: "))
print("You're eligible!")
```

### ✅ Math and Logic Examples

16. **Print first 10 multiples of 4**
```python
i = 1
while i <= 10:
    print(i * 4)
    i += 1
```

17. **Print factorial of 5**
```python
i = 1
fact = 1
while i <= 5:
    fact *= i
    i += 1
print("Factorial:", fact)
```

18. **Print digits of a number**
```python
n = 12345
while n > 0:
    print(n % 10)
    n //= 10
```

19. **Reverse a number**
```python
n = 1234
rev = 0
while n > 0:
    rev = rev * 10 + n % 10
    n //= 10
print("Reversed:", rev)
```

20. **Check if a number is a palindrome**
```python
n = 121
temp = n
rev = 0
while n > 0:
    rev = rev * 10 + n % 10
    n //= 10
print("Palindrome" if rev == temp else "Not palindrome")
```

### ✅ String Handling Examples

21. **Print each character in a string**
```python
text = "Python"
i = 0
while i < len(text):
    print(text[i])
    i += 1
```

22. **Reverse a string**
```python
text = "hello"
rev = ""
i = len(text) - 1
while i >= 0:
    rev += text[i]
    i -= 1
print(rev)
```

23. **Count vowels in a string**
```python
text = "hello world"
i = 0
count = 0
while i < len(text):
    if text[i] in "aeiou":
        count += 1
    i += 1
print("Vowels:", count)
```

24. **Repeat input until user types "yes"**
```python
reply = ""
while reply != "yes":
    reply = input("Do you want to continue? (type yes): ")
```

25. **Print length of input until user types "stop"**
```python
text = ""
while text != "stop":
    text = input("Type something: ")
    print("Length:", len(text))
```

### ✅ List Handling Examples

26. **Print all items in a list**
```python
lst = [1, 2, 3, 4, 5]
i = 0
while i < len(lst):
    print(lst[i])
    i += 1
```

27. **Sum all items in a list**
```python
lst = [5, 10, 15]
i = 0
total = 0
while i < len(lst):
    total += lst[i]
    i += 1
print("Total:", total)
```

28. **Find max in a list**
```python
lst = [5, 3, 9, 2]
i = 1
max_num = lst[0]
while i < len(lst):
    if lst[i] > max_num:
        max_num = lst[i]
    i += 1
print("Max:", max_num)
```

29. **Remove all items from list one by one**
```python
lst = [1, 2, 3]
while lst:
    print("Removing", lst.pop())
```

30. **Count even numbers in a list**
```python
lst = [1, 2, 3, 4, 6]
i = 0
count = 0
while i < len(lst):
    if lst[i] % 2 == 0:
        count += 1
    i += 1
print("Even count:", count)
```

### ✅ Games / Fun Loops

31. **Guess a number game**
```python
secret = 7
guess = -1
while guess != secret:
    guess = int(input("Guess the number: "))
print("Correct!")
```

32. **Print emoji 5 times**
```python
i = 0
while i < 5:
    print("😊")
    i += 1
```

33. **Print increasing stars**
```python
i = 1
while i <= 5:
    print("*" * i)
    i += 1
```

34. **Simple timer from 1 to 5**
```python
import time
i = 1
while i <= 5:
    print(i)
    time.sleep(1)
    i += 1
```

35. **Repeat joke until user laughs**
```python
laugh = ""
while laugh != "haha":
    laugh = input("Say 'haha' to end the joke: ")
print("😂 Finally!")
```

### ✅ Miscellaneous

36. **Sum digits of a number**
```python
n = 123
total = 0
while n > 0:
    total += n % 10
    n //= 10
print("Sum of digits:", total)
```

37. **Convert decimal to binary**
```python
n = 10
binary = ""
while n > 0:
    binary = str(n % 2) + binary
    n //= 2
print("Binary:", binary)
```

38. **Repeat until both numbers are equal**
```python
a, b = 5, 3
while a != b:
    print(a, b)
    a -= 1
    b += 1
```

39. **Print every second letter in string**
```python
text = "Programming"
i = 0
while i < len(text):
    print(text[i])
    i += 2
```

40. **Repeat until list is empty**
```python
items = ["apple", "banana", "cherry"]
while items:
    print("Removing:", items.pop(0))
```
