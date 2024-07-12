# Datatypes: Numbers(Integers, Float), String

## Integers(int)




```python
x=100
type(x)
```




    int




```python
x=654*6734
type(x)
```




    int




```python
print(x)
```

    4404036
    

## Float


```python
x=3.14
print(x)
```

    3.14
    


```python
type(x)
```




    float



# Strings


```python
x="Simplilearn"
print(x)
```

    Simplilearn
    


```python
type(x)
```




    str



# List: Collection of values


```python
x=[14,67,9]
```


```python
print(x)
```

    [14, 67, 9]
    


```python
type(x)
```




    list



### Extracting single values from multiple values in List


```python
#[14,67,9] all have positional index. 
#For instance, 14 has a positional index of 0, 67 has a positional index of 1, and 9 has a positional index of 2. 
# We are going to extract 14 from all the values
```


```python
print(x[0])
```

    14
    


```python
# We are going to extract 67 from all the values
```


```python
print(x[1])
```

    67
    


```python
# We are going to extract 9 from all the values
```


```python
print(x[2])
```

    9
    


```python
#Changing values which is stored within the list with a different number
```


```python
x[2]=67
```


```python
print(x)
```

    [14, 67, 67]
    


```python
x[2]=14
```


```python
print(x)
```

    [14, 67, 14]
    


```python
x[0]=9
```


```python
print(x)
```

    [9, 67, 14]
    

# Tuples


```python
#Tuples involves storing multiple values in a single variable
#In tuple, we use round bracket() instead of square brackets[]
```


```python
x=(4,8,6)
```


```python
print(x)
```

    (4, 8, 6)
    


```python
type(x)
```




    tuple




```python
#The main difference between tuple and list is that tuple is immutable. This means you cannot change the values in tuples.
#changing values in tuples
```


```python
x[2]=5
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[39], line 1
    ----> 1 x[2]=5
    

    TypeError: 'tuple' object does not support item assignment



```python
#The error displayed above indicate that changing values in tuples is impossible
```

### File Pointers


```python
#When dealing with files, we need a variable which point to a particular file. These are called 'File Pointers'
#Advantage of using file pointers:
#When you need to perform various operationson a file, instead of providing a file pathname everytime, can just assign a variable and use that variable.
```


```python
x=open('Class_Work_LearnerNotebook.ipynb','r')
```


```python
type(x)
```




    _io.TextIOWrapper




```python
print(x)
```

    <_io.TextIOWrapper name='Class_Work_LearnerNotebook.ipynb' mode='r' encoding='cp1252'>
    


```python
#Intead of having variables like;
x=5
y=10
z=7,
#We can easily write a simple code to accommodate all the varables
(x,y,z)=5,10,7
```


```python
(x,y,z)=5,10,7
```


```python
print(x,y,z)
```

    5 10 7
    


```python
#If you want the results to display vertically,
```


```python
print(x)
print(y)
print(z)
```

    5
    10
    7
    

### Assigning the same number to multiple variables


```python
#For example, if you want to assign the value 1 to variables x,y, and z
ie, x=1
    y=1
    z=1
#We simply write the following code
(x,y,z)=1,1,1
```


```python
(x,y,z)=1,1,1
print(x,y,z)
```

    1 1 1
    


```python
#We can make the code even more simplier by writing the following code
x=y=z=1
```


```python
x=y=z=1
```


```python
print(x,y,z)
```

    1 1 1
    

# Rules for Naming Variables

### Rule 1:Variable name must begin with an alphabet or an underscore(_)
### Example, abc, _abc


```python
abc=100
```


```python
_abc=100
```

### Rule 2: The first character can be followed by alphabets, numbers or underscore(_)
### Example, a100=100, _a984_=100


```python
a100=100
```


```python
_a984_=100
```


```python
# However, Adding a special charater to the variable will not work
#Example a9874$=100
```


```python
a9874$=100
```


      Cell In[77], line 1
        a9874$=100
             ^
    SyntaxError: invalid syntax
    



```python
#We can see that there is an invalid syntax because the special character($) does not meet the condition for naming variables
```

### Rule 3: Variable names are case sensitive. 
### Capital letters and small letters are treated differently
### Example, a100 is different from A100



```python
a100=100
A100=200
```


```python
print(a100,A100)
```

    100 200
    

### Rule 4: Reserved words cannot be used as a variable names
### Example of reserved words include break, class, and try


```python
break=100
```


      Cell In[83], line 1
        break=100
             ^
    SyntaxError: invalid syntax
    



```python
#As shown above, break has displayed as invalid syntax because it cannot be used as a variable
```


```python
class=8
```


      Cell In[87], line 1
        class=8
             ^
    SyntaxError: invalid syntax
    



```python
#class is shown as invalid syntax because it can be used as a variable in python
```


```python
try=87
```


      Cell In[88], line 1
        try=87
           ^
    SyntaxError: expected ':'
    



```python
# try is shown as invalid because it cannot be used as a variable in python
```

# Performing Arithmetic Operations on Variables(Int, Float)

### Addition


```python
x=20
y=10
```


```python
result=x+y
print(result)
```

    30
    

### Substraction


```python
x=20
y=10
```


```python
result=x-y
print(result)
```

    10
    

### Multiplication


```python
x=20
y=10
```


```python
result=x*y
print(result)
```

    200
    

### Division


```python
x=20
y=10
```


```python
result=x/y
print(result)
```

    2.0
    


```python
#If you do not want your answer to appear as a float, ie 2.0, use a double slash(//)
```


```python
x=20
y=10
```


```python
result=x//y
print(result)
```

    2
    


```python
#If your division for numbers that does not divide each other completely
#For example, if we have result=2/3
```


```python
result=2/3
```


```python
print(result)
```

    0.6666666666666666
    


```python
#The result is 0.6666666666666. If we do not want the result to show as a float, we use double slash //
```


```python
result=2//3
print(result)
```

    0
    

### Finding the Remainder of Arithmetic Operation


```python
#To find the remainder, we use the percentage(%) sign
```


```python
x=20
y=10
```


```python
result=x%y
print(result)
```

    0
    


```python
x=3
y=2
```


```python
result=x%y
print(result)
```

    1
    

### Performing Arithmetic Operation on Floating point numbers


```python
x=3.14
y=5.7
```


```python
result=x/y
print(result)
```

    0.5508771929824562
    


```python
x=3.14
y=5.7
```


```python
result=x+y
print(result)
```

    8.84
    


```python
x=3.14
y=5.7
```


```python
result=x*y
print(result)
```

    17.898
    


```python
x=3.14
y=5.7
```


```python
result=y-x
print(result)
```

    2.56
    

# Performing Arithmetic Operations on  String Variables

### Extracting single variable character from a String


```python
#Var="Simplilearn"
#In case we want find the positional index of each of the letters
#ie S=0, i=1, m=2, p=3, l=4, i=5, l=6, e=7, a=8, r=9, n-10
#To print letter S
```


```python
var="Simplilearn"
print(var[0])
```

    S
    


```python
#Print letter p
```


```python
var="Simplilearn"
print(var[3])
```

    p
    


```python
#Print letter r
```


```python
var="Simplilearn"
print(var[9])
```

    r
    

### Extracting multiple variable character from a String


```python
var="Simplilearn"
```


```python
# Extracting the first 3 characters
```


```python
print(var[0:3])
```

    Sim
    


```python
# Extracting the first 5 characters
```


```python
print(var[0:6])
```

    Simpli
    


```python
#We can also print the first varaible without entering 0 for [0:6] ie [:6]
```


```python
print(var[:6])
```

    Simpli
    


```python
#Printing from the 6th character to the end
```


```python
print(var[6:])
```

    learn
    


```python
#OR without including the end
```


```python
print(var[6:10])
```

    lear
    


```python
#Assuming we want to print all characters
```


```python
print(var[0:])
```

    Simplilearn
    

### Finding the Length of the String


```python
var="Simlpilearn"
```


```python
len(var)
```




    11




```python

```
