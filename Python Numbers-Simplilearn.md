# Numbers in Python

### Integers(int)


```python
num=5
```


```python
type(num)
```




    int




```python
num=23575406471
```


```python
type(num)
```




    int



###  Float


```python
num=5.4
```


```python
type(num)
```




    float



### Complex Numbers


```python
#Complex numbers has two parts. They incude;
#Real complex numbers 
#Imaginary complex numbers
#Complex numbers are stored in floating points
```


```python
num=2+5j
```


```python
type(num)
```




    complex




```python
#Real Complex numbers
```


```python
num.real
```




    2.0




```python
#Imaginary complex numbers
```


```python
num.imag
```




    5.0



### Numbers can also be negative


```python
num=5647.675
```


```python
print(num)
```

    5647.675
    


```python
num
```




    5647.675




```python
type(num)
```




    float



## Performing Arithmetic Operations on Python Numbers

### Addition


```python
num1=10
num2=2
```


```python
print(num1+num2)
```

    12
    

### Subtraction


```python
num1=10
num2=2
```


```python
print(num1-num2)
```

    8
    

### Multiplication


```python
num1=10
num2=2
```


```python
print(num1*num2)
```

    20
    

### Division


```python
num1=10
num2=2
```


```python
print(num1/num2)
```

    5.0
    


```python
#In case you do not want the results to be in a floating point, use two slash(//) signs 
```


```python
num1=10
num2=2
```


```python
print(num1//num2)
```

    5
    


```python
num1=10
num2=3
```


```python
print(num1/num2)
```

    3.3333333333333335
    


```python
#Elinating the floating point
```


```python
num1=10
num2=3
```


```python
print(num1//num2)
```

    3
    

### Raising number to the power of another number in python


```python
#Example, 10 raised to the power 2 is written as 10**2 in python
```


```python
num1=10
num2=2
```


```python
print(num1**num2)
```

    100
    

### Finding the Remainder of a Number


```python
num1=10
num2=2
```


```python
print(num1%num2)
```

    0
    


```python
num1=33
num2=15
```


```python
print(num1%num2)
```

    3
    


```python
num1=10
num2=3
```


```python
print(num1%num2)
```

    1
    

## Python Conversions in Numbers

### Converting String numbers to integers
#### For Example, convert "192" to an integer


```python
x="192"
```


```python
type(x)
```




    str




```python
#"192" is a string number because of the double quotation marks around it
#To convert it to an integer, we apply int to the x value
```


```python
int(x)
```




    192




```python
type(int(x))
```




    int



### Converting the int number to a float number


```python
float(int(x))
```




    192.0




```python
x=float(x)
```


```python
print(x)
```

    192.0
    

### Coverting integers and float to complex numbers


```python
x=192.0
```


```python
x=complex(x)
print(x)
```

    (192+0j)
    


```python
x=100
```


```python
x=complex(x)
print(x)
```

    (100+0j)
    


```python
#Functions to create complex numbers
#Within the complex number, we create real and imaginary numbers
#Example, complex(2,6), where 2 is a real number and 6 is an imaginary number
```


```python
print(complex(2, 6))
```

    (2+6j)
    

## In built Functions that work with Numbers

### 1. Absolute(abs) Function: Returns absolute value of a number


```python
#When real number is positive or negative, the return value is always positive
#For Example, x=-7.5, will return a  positive number when the abs function is applied.
```


```python
x=-7.5
print(abs(x))
```

    7.5
    


```python
y=-5934
print(abs(y))
```

    5934
    

### 2.Exponent(e) Function: This takes a single parameter and returns that parameter as the power of e


```python
# e raised to the power of the parameter you pass to exponent
# ie, e10(e raised to the power 10)
# We import the math library
#Find the value of e raised to the power 10
```


```python
import math
x=10
print(math.exp(x))
```

    22026.465794806718
    


```python
#The value of e
# math.e
#This has a constant value of 2.71
```


```python
math.e
```




    2.718281828459045




```python
#The value of pi
# math.pi
#This has a constant value of 3.14
```


```python
math.pi
```




    3.141592653589793



### 3. Square Root(sqrt) Function: When you pass a value to a function, it returns the square root(sqrt) of that value


```python
# Print the square root of 9
```


```python
print(math.sqrt(9))
```

    3.0
    


```python
# Print the square root of 289
```


```python
print(math.sqrt(289))
```

    17.0
    

### 4. Max() Function: This returns the maximum value of all numbers displayed


```python
#Print the maximum value of these numbers (1,34,489)
```


```python
max(1,34,489)
```




    489




```python
#Print the maximum value of these numbers (100,350,489,1100)
```


```python
max(100,350,489,1100)
```




    1100



### 5. Min() Function: This returns the minimum value of all numbers displayed


```python
# Print the minimum number of these values(1,34,4986,3254,687)
```


```python
min(1,34,4986,3254,687)
```




    1




```python
# Print the minimum number of these values(1234,3443,4986,3254,8687)
```


```python
min(1234,3443,4986,3254,8687)
```




    1234



## What are Lists?

### A List is a collection of data. It can hold values of multiple data types
### Example list x can contain, 1,89,A,Hey,0, B 
### X=[1,89,A,Hey,0,B]


```python
#All Lists have positional indexes, the positional index of 1 ia 0, 89 is 1, A is 2, Hey is 3, 0 is 4 and B is 5
```

#### Creating Lists of Integers


```python
num=[1,2,3,4]
print(num)
```

    [1, 2, 3, 4]
    

#### Creating lists for single characters


```python
letter=["a","b","c","d"]
```


```python
print(letter)
```

    ['a', 'b', 'c', 'd']
    

#### Creating a list for strings


```python
stg=["get","your","Chelsea","jersey", "now"]
```


```python
print(stg)
```

    ['get', 'your', 'Chelsea', 'jersey', 'now']
    

#### Creating a list containing a combination of different datatypes


```python
mix=[1,6,"get","your","chelsea","jersey","now"]
```


```python
print(mix)
```

    [1, 6, 'get', 'your', 'chelsea', 'jersey', 'now']
    

#### Creating a list containing two or more lists(matrices)


```python
mat=[[1,2],["a","b"]]
```


```python
print(mat)
```

    [[1, 2], ['a', 'b']]
    


```python
mat=[[1,2],["a","b"],["chelsea","football","club"]]
```


```python
print(mat)
```

    [[1, 2], ['a', 'b'], ['chelsea', 'football', 'club']]
    

## Accessing Elements in Lists


```python
#In accessing elements in lists, we use positional index of the element
#Extract "chelsea" from the lists
```


```python
print(mix)
```

    [1, 6, 'get', 'your', 'chelsea', 'jersey', 'now']
    


```python
mix[4]
```




    'chelsea'




```python
#Extract "jersey" from the list
```


```python
mix[5]
```




    'jersey'



#### Similarly, we can use negative(-) indices to access the elements in the list


```python
#The negative sign allow us to count the elements from backwards
#Extract "jersey" from the list using the negativ(-) sign 
```


```python
mix[-2]
```




    'jersey'




```python
#In this case, we have been able to access "jersey" by counting from backwards from "now", which is -2
```


```python
#NOTE: If we count list from the beginning (front), it starts with 0,
#However, if we count a list from backwards, it starts with -1
```

### Accessing a Range of Elements


```python
print(mix)
```

    [1, 6, 'get', 'your', 'chelsea', 'jersey', 'now']
    


```python
#Extract the first four elements from mix
```


```python
mix[0:4]
```




    [1, 6, 'get', 'your']




```python
#Extract the first two elements from mix
```


```python
mix[:2]
```




    [1, 6]




```python
#Extract the all elements from mix
```


```python
mix[:7]
```




    [1, 6, 'get', 'your', 'chelsea', 'jersey', 'now']




```python
#Extract all elements from the starting position of the list "your"

mix[3:]
```




    ['your', 'chelsea', 'jersey', 'now']




```python
#Extract all elements from the starting position of the list "get" and end at "jersey"

mix[2:6]
```




    ['get', 'your', 'chelsea', 'jersey']




```python
#OR you can count it from backwards

mix[2:-1]
```




    ['get', 'your', 'chelsea', 'jersey']




```python
#Extract "chelsea" and "jersey"

mix[4:-1]
```




    ['chelsea', 'jersey']




```python
mix[4:6]
```




    ['chelsea', 'jersey']



### Extracting every second element of list


```python
print(mix)
```

    [1, 6, 'get', 'your', 'chelsea', 'jersey', 'now']
    


```python
#Extract every second element of the list
```


```python
mix[::2]
```




    [1, 'get', 'chelsea', 'now']




```python
#Extract every first element of the list

mix[::1]
```




    [1, 6, 'get', 'your', 'chelsea', 'jersey', 'now']




```python
#Extract every third element of the list

mix[::3]
```




    [1, 'your', 'now']



### Printing lists in reverse order


```python
print(mix)
```

    [1, 6, 'get', 'your', 'chelsea', 'jersey', 'now']
    


```python
#Print a reverse version of mix

mix[::-1]
```




    ['now', 'jersey', 'chelsea', 'your', 'get', 6, 1]



## Operations on Lists

### Multiplication


```python
#Create a list of 100 zeros

z=[0]*100
print(z)
```

    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
    


```python
#Create a list of 100 zeros,200 ones, and 300 fives

k=[[0]*100,[1]*200,[5]*300]
print(k)
```

    [[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1], [5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5, 5]]
    

### Concatenating(Addition)


```python
#Create a list to concatenate the two list that we previously created (ie letter, and stg(string))

print(letter)
```

    ['a', 'b', 'c', 'd']
    


```python
print(stg)
```

    ['get', 'your', 'Chelsea', 'jersey', 'now']
    


```python
#Concatenate letter and stg

conc=letter+stg
print(conc)
```

    ['a', 'b', 'c', 'd', 'get', 'your', 'Chelsea', 'jersey', 'now']
    

### Giving a string as in an argument to this function list and make each element of the string as saparate element in a list


```python
# Every letter string in the list becomes a single element in the lis var

var=list("hey there")
print(var)
```

    ['h', 'e', 'y', ' ', 't', 'h', 'e', 'r', 'e']
    

### Picking one or more elements ina list and storing them in different variable


```python
#Using the list num previously created

print(num)
```

    [1, 2, 3, 4]
    


```python
#We want the first element[1] of list num to be in a variable "one" and 
#want the rest of the elements [2,3,4] to be stored in another list called "other"

one,*other=num
print(one)
print(other)
```

    1
    [2, 3, 4]
    


```python
#In this case, element [1] has been stored as one, and elements[2,3,4] has been stored as other
```

## Methods in Lists

### Append():  Assigning or adding an element to a list


```python
#Append 6 to the num list

num.append(6)
print(num)
```

    [1, 2, 3, 4, 6]
    

### Extend(): Adding multiple elements to a list


```python
print(num)
```

    [1, 2, 3, 4, 6]
    


```python
#Add stg(string) to the num list
num.extend(stg)
```


```python
print(stg)
```

    ['get', 'your', 'Chelsea', 'jersey', 'now']
    


```python
print(num)
```

    [1, 2, 3, 4, 6, 'get', 'your', 'Chelsea', 'jersey', 'now']
    

### Insert(): Inserting elements in between the list


```python
#Insert 20, and "Cole Palmer" in between the codes

num.insert(7, "Cole Palmer")

print(num)
```

    [1, 2, 3, 4, 6, 'get', 'your', 'Cole Palmer', 'Chelsea', 'jersey', 'now']
    

### Remove(): This removes an element from a list


```python
#Remove Chelsea from the list

num.remove("Chelsea")

print(num)
```

    [1, 2, 3, 4, 6, 'get', 'your', 'Cole Palmer', 'jersey', 'now']
    

### Sort(): Sorting elements in such a way that it is arranged in order


```python
#Lets create a variable called char1
#var1=['b','f','a','q','r']

var1=['b','f','a','q','r']

print(var1)

```

    ['b', 'f', 'a', 'q', 'r']
    


```python
#Sort Var1

var1.sort()

print(var1)
```

    ['a', 'b', 'f', 'q', 'r']
    

## Build-in Functions with lists


```python
#Lets create a new list

x=[9,17,14,4,90,55]
```

### len():Finding the length of your list


```python
#Find the len() of x=[9,17,14,4,90,55]

len(x)
```




    6



### min(): Finding the minimum number of all elements in the list


```python
#Find the minimum number of all elements

min(x)
```




    4



### max(): Finding the maximum number of all elements in the list


```python
#Find the maximum number of all elements

max(x)
```




    90



### sum(): Finding the sum of all elements present in a list


```python
#Find the sum of all elements in the list

sum(x)
```




    189



### Finding the average number of elements in a list


```python
average=sum(x)/len(x)
```


```python
print(average)
```

    31.5
    


```python

```
