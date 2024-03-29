Here's the documentation for the provided Python code:

---

## 1. ARITHMETIC OPERATION

### Simple Arithmetic

```python
a = 5
b = 6
c = a + b
print(c)
```

### Simple Arithmetic - Get input from User (+,-,*,%)

```python
a = float(input("Enter the value of a: "))
b = float(input("Enter the value of b: "))
add = a + b
print(add)
```

```python
a = int(input("Enter the value of a: "))
b = int(input("Enter the value of b: "))
add = a + b
sub = a - b
mult = a * b
div = a / b
mod = a % b
print("ADD:", add)
print("Sum: {0}, Diff: {1}, Mult: {2}, Div:{3}, Mod:{4}".format(add, sub, mult, div, mod)) #Print using Format
```


### Simple Arithmetic - Get input from User (power)

```python
a = 2
b = 3
power = a ** b  # Power
print(power)
```

## 2. STRINGS

### Create String

```python
a = 'Python'
b = "Bootcamp"
print(a + b)
```

### Length of String

```python
a = "Champ"
print(len(a))
```

```python
a = "S"
b = a * 5
print(b)
```

### String Index

```python
a = "champ"
print(a[3])     # identifying the element based on index
print(a[2:])    # Grab the remaining elements except up to the Index
print(a[:2])    # Grab the elements up to the Index
print(a[-1])    # Grab the Last element
print(a[:-1])   # Grab the elements except the last element
print(a[::2])   # Grab everything with 2 steps
print(a[::-1])  # Print string backwards
```

### String Functions

```python
a = "Master Class"
print(a.upper())   # Changing to Upper case
print(a.lower())   # Changing to Lower case
```

```python
b = a.split()  # Splitting String
print(b)
print(b[1])     # Printing the splitting string based on Index
```

```python
c = "ElonMusk,SteveJobs,BillGates"
d = c.split(",")  # Splitting string based on Delimiter
print(d)
print(d[1])
```

```python
a = "Master Class"
print(f"Welcome to Python {a} !")  # Formatting string Literals
```

## 3. LIST

### Create List

```python
a = [1, 2, 3, 4, 5]
b = ["Champ", 21, 99.5]
print(a, b)
```

### Length of List

```python
print(len(b))       # Length of List
```

```python
print(b[0])         # Locate list element based on Index
```

```python
print(a[1:])        # print elements except 1st
```

```python
print(a[:2])        # Print elements up to 2nd element
```

```python
print(a + b)        # Concatenate 2 lists
```

### Modifying Lists

```python
a = [1, 2, 3, 4, 5]
a.append(6)         # inserting new elements to the existing list
print(a)
```

```python
a = [1, 2, 3, 4, 5]
a.reverse()         # Reverse list
print(a)
```

```python
print(min(a))       # Minimum
print(max(a))       # Maximum
```

```python
from random import shuffle
shuffle(a)
print(a)
```

### Nested List (Matrix)

```python
a = [1, 2, 3]
b = [4, 5, 6]
c = [a, b]          # Nested List Matrix
print(c)
print(c[0])         # Printing row
print(c[0][0])      # Printing 1st element
```

## 4. DICTIONARIES

### Creating Dictionary: Key & Value

```python
a = {"Name": "Elon", "Age": 50, "Company": ["SpaceX", "Tesla"]}
print(a)
```

```python
a = {"Name": "Elon", "Age": 50, "Company": ["SpaceX", "Tesla"]}
print(a["Name"])    # Printing value based on its Key
```

```python
a["Age"] = 51      # Changing values
print(a)
```

```python
b = {"Climate": {"Condition": {"Temperature": "38 Degree", "Humidity": "70 Percentage"}}}
print(b["Climate"]["Condition"]["Humidity"])
```

```python
print(a.keys())    # Printing Keys of the Dictionaries
print(a.values())  # Printing Values of the Dictionaries
print(a.items())   # Printing Tuple of all items
```

## 5. TUPLES

### Creating Tuples

```python
a = ("Champ", 21, 99.5)
print(a)
```

```python
print(len(a))      # Length of tuple
```

```python
print(a[0])        # Printing elements from tuple via index
```

```python
print(a.index("Champ"))  # Getting Index of Elements
```

## 6. SETS

### Creating Set

```python
a = set()
print(a)
```

```python
a.add("Champ")
print(a)
```

```python
a.add(30)
print(a)
```

```python
b = ["Champ", 21, 99.5]
print(set(b))
```

## 7. BOOLEAN

### Creating Boolean

```python
a = True
print(a)
```

### Comparison Operations

```python
a = 10
b = 5
c = 15

print(a == b)
print(a != b)
print(a <= b)
print(a >= b)
```

## 8. Python Statements

### If Statement

```python
a = True
if a:
    print("Positive")
else:
    print("negative")
```

### For Loop

```python
a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 

10]
for i in a:
    print(i)
```

```python
a = [i for i in 'Champ']
print(a)
```

### Odd & Even Number

```python
a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
for i in a:
    if i % 2 == 0:
        print(i, "Even Number")
    else:
        print(i, "Odd Number")
```

### String - For Loop

```python
for a in "Hello all":
    print(a)
```

### Dictionary - For Loop

```python
a = {"Name": "Elon", "Age": 50, "Company": ["SpaceX", "Tesla"]}
for k, v in a.items():
    print(k)
    print(v)
```

### While Loop

```python
a = 0
while a < 11:
    print(a)
    a += 1  # a=a+1
```

### While Loop - Break & Continue

```python
a = 0
while a < 10:
    print(a)
    a += 1
    if a == 5:
        print("a is equal to 5")
        break
    else:
        print("Continueeee")
        continue
```

### Range Function

```python
for a in range(6):
    print(a)
```

```python
for a in range(1, 10, 1):
    print(a)
```

```python
for a in range(10, 0, -3):
    print(a)
```

```python
a = [i**2 for i in range(0, 5)]
print(a)
```

```python
a = [i for i in range(10) if i % 2 == 0]
print(a)
```

### Enumerate

```python
a = 0
for i, a in enumerate("Hello Champ"):
    print(i, a)
```

### Zip

```python
a = ["Name", "Age", "Country"]
b = ["Champ", 27, "India"]
print(list(zip(a, b)))
```

## 9. FUNCTION

### Initializing & Calling Basic Function

```python
def welcome():
    print("Hello guyz Welcome to Python Bootcamp !!!")
welcome()
```

### Initializing & Calling Basic Function - With Argument

```python
def welcome(a):
    print("Hello {0},Welcome to Python Bootcamp !!!".format(a))
welcome("Champ")
```

### Print & Return

```python
def add(a, b):
    add = a + b
    print("Sum of {0} and {1} is {2}".format(a, b, add))
def addR(a, b):
    add = a + b
    return add

ans = addR(45, 5)
final = ans * 500
print(final)
```

### Practice Project - Extracting Prime Numbers

```python
def check(numbers):
    primeNumber = []
    for number in numbers:
        if number > 1:
            for i in range(2, int(number/2)+1):
                if (number % i) == 0:  # If number is divisible by any number between 2 and number / 2, it is not prime
                    print(number, "is not a prime number")
                    break
            else:
                print(number, "is a prime number")
                primeNumber.append(number)
        else:
            pass
    return primeNumber

check([2, 3, 4, 5, 6, 7, 8, 9])
```

## 10. MAP FUNCTION

### Map a function to an iterable object

```python
def cubeFn(num):
    return num**3

a = [1, 2, 3, 4, 5]
print(list(map(cubeFn, a)))
```

## 11. FILTER FUNCTION

### Yields items of iterable in which function is true

```python
def evenFn(num):
    return num % 2 == 0

a = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
print(list(filter(evenFn, a)))
```

## 12. LAMBDA FUNCTION

### To create anonymous functions, without using def

```python
def cubeFn(num):
    return num**3
cubeFn(6)
```

```python
cubefn = lambda num: num**3
cubefn(5)
```

## 13. *ARGS AND **KWARGS

### *Args

```python
def addR(*argg):
    return sum(argg)
addR(10, 20, 30, 40, 52, 75, 8, 5, 26, 15)
```

### **Kwargs

```python
def func(**kwargs):
    if 'name' in kwargs:
        print("My Name is {0}".format(kwargs['name']))
    if 'age' in kwargs:
        print("My Age is {0}".format(kwargs['age']))
    else:
        print("No Key Found")

func(name='champ', age=24, marks=99)
```

## 14. OBJECT ORIENTED PROGRAMMING

### Class

```python
class Student:
    print("Hello All")

x = Student()  # Object Instantiation
print(type(x))
```

### Class Object Attribute

```python
class Student:
    year = '2021'
    print("Hello All")

x = Student()
print(x.year)
```

### Attribute of an Object

```python
class Student:
    def __init__(self, name):
        self.name = name

elon = Student(name='Elon Musk')
print(elon.name)
```

## 15. PYTHON DECORATORS

### Functions which modify the functionality of another function/Class

```python
def decoratorFunc(welcome):  # 2. Decorator
    def a():  # 3. can access the outer local functions like in this case "welcome"
        print("Start")
        welcome()  # 4.calling actual fn.
        print("End")
    return a

def subFunc():  # 1. subFunc inside the decorator to control behavior
    print("Sub fn")

subFunc = decoratorFunc(subFunc)

subFunc()
```

## 16. PYTHON GENERATORS

### To generate as we go along, instead of holding everything in memory

```python
def square(n):
    for i in range(n):
        yield i**2

for n in square(10):
    print(n)
```

## 17. PYTHON MODULES & LIBRAR

IES

### Math Library

```python
import math
print(math.pi)
```

### Working with Files

```python
f = open("welcome.txt", "r")
print(f.read())
f.close()
```

### File Handling using Pandas

```python
import pandas as pd
data = pd.read_csv('data.csv')
print(data.shape)
print(data.describe())
print(data.head(5))
```

### Working with Directories

```python
import os
print(os.getcwd())  # current working directory
print(os.listdir())
os.mkdir("Junk")
```

### Time

```python
import time
print(time.time())  # time since epoch
```

### Date & Time

```python
import datetime
x = datetime.datetime.now()
print(x)
```

This document provides a structured overview of Python concepts, including arithmetic operations, strings, lists, dictionaries, tuples, sets, boolean operations, loops, functions, object-oriented programming, decorators, generators, and modules/libraries. Each section includes code examples and explanations for better understanding.
