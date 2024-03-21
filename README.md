# All of syntax of python in one file
Anyone can learn from this file and that would be the easy and fastest way to learn python programming. Start learnin...
All of practice code save in python.ipynb, hi programmer you can practice with this file

<br/>
<br/>
###  ARITHMETIC OPERATION

#### Simple Arithmetic

``` python
a=5
b=6
c=a+b
print(c)
```


``` python
a = float(input("Enter the value of a: "))
b = float(input("Enter the value of b: "))
add=a+b
print(add)
```


``` python
a = int(input("Enter the value of a: "))
b = int(input("Enter the value of b: "))
add=a+b
sub=a-b
mult=a*b
div=a/b
mod=a%b
print("ADD:",add)
print("Sum: {0}, Diff: {1}, Mult: {2}, Div:{3}, Mod:{4}".format(add,sub,mult,div,mod)) #Print using Format
```



``` python
print('{0:<4} | {1:^4} | {2:^4} | {3:>4}'.format('Sum','Diff','Mult','Div'))
print('{0:<4} | {1:^4} | {2:^4} | {3:>4}'.format(add,sub,mult,div))
```

#### Simple Arithmetic - Get input from User (power)


``` python
a=2
b=3
power=a**b #Power
print(power)
```

##  STRINGS

#### Create String


``` python
a = 'Python'
b = "Bootcamp"
print(a+b)
```

#### Length of String

``` python
a="Champ"
print(len(a))
```

``` python
a="S"
b=a*5
print(b)
```

### String Index

``` python
a="champ"
print(a[3]) #identifing the element based on index
print(a[2:]) #Grab the remaing elements except upto the Index
print(a[:2]) #Grab the elements upto the Index
print(a[-1]) #Grab the Last element
print(a[:-1]) #Grab the elements except last element
print(a[::2]) #Grab everything with 2 steps
print(a[::-1]) #Print string backwards
```

### String Functions

``` python
a="Master Class"
print(a.upper()) #Changing to Upper case
print(a.lower()) #Changing to Lowerb= a.split() case
```
#### Splitting String

``` python
b= a.split() 
print(b)
print(b[1]) 
```

``` python
c="ElonMusk,SteveJobs,BillGates"
d=c.split(",") #Splitting string based on Delimitter
print(d)
print(d[1])
```

``` python
a="Master Class"
print(f"Welcome to Python {a} !") #Formatting string Literals
```

##  LIST

### Create List

``` python
a = [1,2,3,4,5]
b = ["Champ",21,99.5]
print(a,b)
print(len(b)) #Length of List
print(b[0]) #Locate list element based on Index
print(a[1:]) #print elements except 1st
print(a[:2]) #Print elements upto 2nd element
print(a+b) #Concatenate 2 list
```

``` python
a = [1,2,3,4,5]
a.append(6) #inserting new elements to the existing list
print(a)
```

``` python
a = [1,2,3,4,5]
a.reverse() #Reverse list
print(a)
print(min(a)) #Minimum
print(max(a)) #Maximum 
```

``` python
a = [1,2,3,4,5]
from random import shuffle
shuffle(a)
a
```

``` python
a=[1,2,3]
b=[4,5,6]
c=[a,b] #Nested List Matrix
print(c)
print(c[0]) #Printing row
print(c[0][0]) #Printing 1st element 
```

##  DICTIONARIES

### Creating Dictionary : Key & Value

``` python
a = {"Name":"Elon","Age":50,"Company":["SpaceX","Tesla"]}
a
```

``` python
a = {"Name":"Elon","Age":50,"Company":["SpaceX","Tesla"]}
print(a["Name"]) #Printing value based on its Key
a["Age"]= 51 #Changing values
a
```

``` python
b={"Climate":{"Condition":{"Temperature":"38 Degree","Humidity":"70 Percentage"}}}
print(b["Climate"]["Condition"]["Humidity"])
```

``` python
print(a.keys()) #Printing Keys of the Dictionaries
print(a.values()) #Printing Values of the Dictionaries
print(a.items()) #Printing Tuple of the all items
```

## Practice Project - Extracting Prime no. {#practice-project---extracting-prime-no}

``` python
def check(numbers):
    primeNumber = []
    for number in numbers:
      if number>1:
        for i in range(2, int(number/2)+1):
          if (number % i) == 0:#If number is divisible by any number between 2 and number / 2, it is not prime
              print(number, "is not a prime number")
              break
        else:
          print(number, "is a prime number")
          primeNumber.append(number)
      else:
        pass
    return primeNumber
```

``` python
check([2,3,4,5,6,7,8,9])
```

## Map Function - Map a function to an iterable object {#10-map-function---map-a-function-to-an-iterable-object}

``` python
def cubeFn(num):
    return num**3
```

``` python
a = [1,2,3,4,5]
list(map(cubeFn,a))
```


### Working with Files

``` python
f = open("welcome.txt", "r")
print(f.read())
f.close()
```

``` python
f = open("welcome.txt", "r")
print(f.read(5))
f.close()
```

``` python
f = open("welcome.txt", "r")
print(f.readline())
f.close()
```

``` python
f = open("welcome.txt", "r")
for x in f:
  print(x)
```



### File Handling using Pandas

``` python
!pip install pandas
```

``` python
import pandas as pd
data = pd.read_csv('data.csv')
print(data.to_string()) 
```

``` python
import pandas as pd
data = pd.read_csv('data.csv')
print(data.shape)
print(data.describe())
print(data.head(5)) 
```


## Don't waste your time, start learning with python.ipynb file
