# 📚 Questions for ID: 5bad24a1a2da6b554b878132

## :question: Question 1 (Order: 1)

<p>Write a function to find and print the square of an entered number x.</p>


### 💻 Solution (python):

```python
x = int(input())

def find_square(x):
  print (x * x)

find_square(x)
```

---

## :question: Question 2 (Order: 2)

<p>Write a program to define a two functions, one is for finding a square of an entered numbers(x and y) and second is for finding the sum of the square of a two entered numbers(x and y) and print the result of sum.</p>


### 💻 Solution (python):

```python
x = int(input())
y = int(input())

def find_square(num):
  return num * num

def find_sum(num1, num2):
  return num1 + num2
  
print(find_sum(find_square(x), find_square(y)))
```

---

## :question: Question 3 (Order: 3)

<p>Write a function to read a two entered values and store them in reverse order as a list. The output will display the values in a list.</p>


### 💻 Solution (python):

```python
num1 = int(input())
num2 = int(input())

def reversenum(num1,num2):
    return [num2,num1]
    
print(reversenum(num1,num2))
```

---

## :question: Question 4 (Order: 4)

<p>Write a function to calculate and print the area and perimeter of a square against an entered side value.</p>
<p><strong>Hint:</strong> Area = square of side, perimeter = 4 * side</p>


### 💻 Solution (python):

```python
side = int(input())

def calculate(side):
  print("Area: " + str(side * side))
  print("Perimeter: " + str(4 * side))
  
calculate(side)
```

---

## :question: Question 5 (Order: 5)

<p>Write a function to check if an entered number is odd or even and returns 'Odd', if number is odd otherwise returns 'Even'. The output will display the result as 'Odd' or 'Even' according to the returns of function.</p>


### 💻 Solution (python):

```python
num = int(input())

def Find_odd_or_even(num):
  if (num % 2 == 0):
    return "Even"
  else:
    return "Odd"
  
print(Find_odd_or_even(num))
```

---

## :question: Question 6 (Order: 6)

<p>Write a program to find and print a factorial of an entered number by using function.</p>


### 💻 Solution (python):

```python
num = int(input())

def find_factorial(num):
  if (num == 1):
    fact = 1
  else:
    fact = num * find_factorial(num - 1)
  return fact

print(find_factorial(num))
```

---

## :question: Question 7 (Order: 7)

<p>Write a function to find the largest number of an entered three numbers (x,y and z). The output will display the largest number.</p>


### 💻 Solution (python):

```python
x = int(input())
y = int(input())
z = int(input())

def Find_largest_of_two( x, y ):
    if x > y:
        return x
    return y
  
def Find_largest_of_three( x, y, z ):
    return Find_largest_of_two( x, Find_largest_of_two( y, z ) )

print(Find_largest_of_three(x, y, z))
```

---

## :question: Question 8 (Order: 8)

<p>Write a function to find and print the sum of all the numbers of a given list [4, 5, 6, 3, 7, 9].</p>


### 💻 Solution (python):

```python
num = [4, 5, 6, 3, 7, 9]
def Add_list(num):
    total = 0
    for x in num:
        total = total + x
    return total
print(Add_list(num))
```

---

## :question: Question 9 (Order: 9)

<p>Write a function to check whether an entered number is in a given range and print 'The number is in the given range.' if an entered number is in given range otherwise print 'The number is outside the given range.'.</p>


### 💻 Solution (python):

```python
num = int(input())
lower = int(input())
upper = int(input())

def check_number(num,lower,upper):
  found = False
  for i in range(lower, upper):
    if (i == num):
      found = True
      break
  if(found):
    print( "The number is in the given range.")
  else :
    print("The number is outside the given range.")

check_number(num, lower, upper)
```

---

## :question: Question 10 (Order: 10)

<p>Write a function which is used to print a dictionary (d) where the keys are numbers between 1 and 10 (both included) and the values are square of keys.</p>
<p><strong>Note:</strong> The output will display the resulted dictionary.</p>


### 💻 Solution (python):

```python
def print_dict():
	d=dict()
	for i in range(1, 11):
          d[i]= i * i
	print(d)
print_dict()
```

---

## :question: Question 11 (Order: 11)

<p>Write a function which is used to print a dictionary (d) where the keys are numbers between 1 and 5 (both included) and the values are factorial of keys. </p>
<p><strong>Note:</strong> The output will display the resulted dictionary.</p>


### 💻 Solution (python):

```python
def find_factorial(num):
    if (num == 1):
        return 1
    return num * find_factorial(num - 1)

def print_dict():
    d=dict()
    for num in range(1, 6):
        d[num] = find_factorial(num)
    print(d)

print_dict()
```

---

## :question: Question 12 (Order: 12)

<p>Write a program to compute the below function for an entered number, n and print the result of it.</p>
<p>f(n)=f(n-1)+100 ,where f(0)=1</p>


### 💻 Solution (python):

```python
n = int(input())

def calculateFunction(n):
    if n==0:
        return 1
    else:
        return calculateFunction(n - 1) + 100

print(calculateFunction(n))
```

---

## :question: Question 13 (Order: 13)

<p>Write a binary search function which is used to search an entered number in the given sorted list (s_list) and returns the index position of the number, if found otherwise return Not found. </p>
<p>s_list = [3, 4, 6, 7, 8, 9, 11, 15, 18]</p>
<p><strong>Note:</strong> The output will display the index position of an entered number or Not found against returns of function.</p>


### 💻 Solution (python):

```python
import math
s_list = [3, 4, 6, 7, 8, 9, 11, 15, 18]
num = int(input())

def binary_search(s_list, element):
    bottom = 0
    top = len(s_list) - 1
    index = False
    while (top >= bottom and index == False):
        mid = int(math.floor((top + bottom) / 2.0))
        if (s_list[mid] == element):
            index = mid
        elif (s_list[mid] > element):
            top = mid - 1
        else:
            bottom = mid + 1
    if(index):
        return index
    else:
        return "Not found"

print(binary_search(s_list, num))
```

---

