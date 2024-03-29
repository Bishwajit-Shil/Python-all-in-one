
# Python Basics Documentation

## 1. Arithmetic Operations

### Simple Arithmetic

Performing basic arithmetic operations.

```python
a = 5
b = 6
c = a + b
print(c)  # Output: 11
```

### Simple Arithmetic - Get Input from User

```python
a = float(input("Enter the value of a: "))
b = float(input("Enter the value of b: "))
add = a + b
print(add)
```

### Arithmetic Operations with User Input

```python
a = int(input("Enter the value of a: "))
b = int(input("Enter the value of b: "))
add = a + b
sub = a - b
mult = a * b
div = a / b
mod = a % b
print("ADD:", add)
print("Sum: {0}, Diff: {1}, Mult: {2}, Div: {3}, Mod: {4}".format(add, sub, mult, div, mod))
```

## 2. Strings

### Create String

Creating and concatenating strings.

```python
a = 'Python'
b = "Bootcamp"
print(a + b)  # Output: PythonBootcamp
```

### Length of String

```python
a = "Champ"
print(len(a))  # Output: 5
```

### String Indexing

```python
a = "champ"
print(a[3])    # Output: m
print(a[2:])   # Output: amp
print(a[:2])   # Output: ch
print(a[-1])   # Output: p
print(a[:-1])  # Output: cham
print(a[::2])  # Output: cm
print(a[::-1]) # Output: pmahc
```

### String Functions

```python
a = "Master Class"
print(a.upper())       # Output: MASTER CLASS
print(a.lower())       # Output: master class
b = a.split()          # Output: ['Master', 'Class']
print(b)
print(b[1])            # Output: Class
```

## 3. Lists

### Create List

Creating lists and performing basic operations on them.

```python
a = [1, 2, 3, 4, 5]
b = ["Champ", 21, 99.5]
print(a, b)
print(len(b))          # Output: 3
print(b[0])            # Output: Champ
print(a[1:])           # Output: [2, 3, 4, 5]
print(a[:2])           # Output: [1, 2]
print(a + b)           # Output: [1, 2, 3, 4, 5, 'Champ', 21, 99.5]
```

### List Operations

```python
a = [1, 2, 3, 4, 5]
a.append(6)            # Output: [1, 2, 3, 4, 5, 6]
a.reverse()            # Output: [6, 5, 4, 3, 2, 1]
print(min(a))          # Output: 1
print(max(a))          # Output: 6
```

### Nested Lists

```python
a = [1, 2, 3]
b = [4, 5, 6]
c = [a, b]             # Output: [[1, 2, 3], [4, 5, 6]]
print(c)
print(c[0])            # Output: [1, 2, 3]
print(c[0][0])         # Output: 1
```

## 4. Dictionaries

### Creating Dictionary: Key & Value

```python
a = {"Name": "Elon", "Age": 50, "Company": ["SpaceX", "Tesla"]}
print(a)
print(a["Name"])       # Output: Elon
a["Age"] = 51          # Changing values
print(a)
```

### Accessing Dictionary Items

```python
b = {"Climate": {"Condition": {"Temperature": "38 Degree", "Humidity": "70 Percentage"}}}
print(b["Climate"]["Condition"]["Humidity"])  # Output: 70 Percentage
print(a.keys())       # Output: dict_keys(['Name', 'Age', 'Company'])
print(a.values())     # Output: dict_values(['Elon', 51, ['SpaceX', 'Tesla']])
print(a.items())      # Output: dict_items([('Name', 'Elon'), ('Age', 51), ('Company', ['SpaceX', 'Tesla'])])
```

## 5. Tuples

### Creating Tuples

```python
a = ("Champ", 21, 99.5)
print(a)              # Output: ('Champ', 21, 99.5)
print(len(a))         # Output: 3
print(a[0])           # Output: Champ
print(a.index("Champ"))  # Output: 0
```

## 6. Sets

### Creating Set

```python
a = set()
a.add("Champ")
print(a)              # Output: {'Champ'}
a.add(30)
print(a)              # Output: {'Champ', 30}
```

## 7. Boolean

### Creating Boolean

```python
a = True
print(a)              # Output: True
```

### Boolean Operations

```python
a = 10
b = 5
c = 15
print(a > b)          # Output: True
print(a == b)         # Output: False
print(a != b)         # Output: True
print(a <= b)         # Output: False
print(a >= b)         # Output: True
```

## 8. Python Statements

### If Statement

```python
a = True
if a:
    print("Positive")
else:
    print("Negative")
```

### For Loop

```python
a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
for i in a:
    print(i)
```

### Odd & Even Numbers

```python
a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
for i in a:
    if i % 2 == 0:
        print(i, "Even Number")
    else:
        print(i, "Odd Number")
```

### While Loop

```python
a = 0
while a < 11:
    print(a)
    a += 1
```

### Range Function

```python
for a in range(6):
    print(a)
```

### Enumerate Function

```python
for i, a in enumerate("Hello Champ"):
    print(i, a)
```

### Zip Function

```python
a = ["Name", "Age", "Country"]
b = ["Champ", 27, "India"]
print(list(zip(a, b))) 
