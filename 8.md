# 📚 Questions for ID: 5bae1a44d52cb8455aa638dc

## :question: Question 1 (Order: 1)

<p>Write a program to make a new list which stores the squares of every elements of previous list which containing 5, 6, 2, 1, 4, 3 and print the new list.</p>


### 💻 Solution (python):

```python
num = [5, 6, 2, 1, 4, 3]
squares = []
for i in num:
  squares.append(i * i)
print (squares)
```

---

## :question: Question 2 (Order: 2)

<p>Write a program to print the multiplication table of an entered number using for loop in format as (index x entered_number) = result, where index=1 to 10.</p>


### 💻 Solution (python):

```python
number = int(input())
for i in range(1, 11):
  print(str(i) + " x " + str(number) + " = " + str(i * number))
```

---

## :question: Question 3 (Order: 3)

<p>Write a program to print the multiples of 10 in the range of 1 and 100.</p>


### 💻 Solution (python):

```python
for i in range(1, 101):
  if(i % 10 == 0):
    print(i)
```

---

## :question: Question 4 (Order: 4)

<p>Write a program to print the number series 2, 4, 8, 16, 32, 64, 128, 256, 512, 1024 as a list.</p>


### 💻 Solution (python):

```python
num_list = []
number = 1
while(number < 1024):
  number = number * 2
  num_list.append(number)
print(num_list)
```

---

## :question: Question 5 (Order: 5)

<p>Write a program to print the number series 0, 5, 10, 15, 30, 35, 70, 75, 150, 155, 310, 315, 630, 635 as a list.</p>


### 💻 Solution (python):

```python
num_list = []
number = 0
while (number <= 630):
    num_list.append(number)
    number = number + 5
    num_list.append(number)
    number = number * 2
print(num_list)
```

---

## :question: Question 6 (Order: 6)

<p>Write a program to print the month name with its sequence number in format as "1 January and so on" by using a list of months in order.</p>


### 💻 Solution (python):

```python
months = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
for n in range(12):
    print(str(n + 1) + "  " + months[n])
```

---

## :question: Question 7 (Order: 7)

<p>Write a program to find an average of 10 entered number and print the average value.</p>
<p><strong>Note:</strong> Take 10 user input by using for loop.</p>


### 💻 Solution (python):

```python
total = 0
for i in range(10):
  x = float(input())
  total = total + x
average = total / 10.0
print(average)
```

---

## :question: Question 8 (Order: 8)

<p>Write a program to take  an integer inputs from the user until the user presses q and print the average value and product of all numbers.The output format should be required as below.</p>
<p>Average is &lt;average_value&gt;</p>
<p>Product of all number is &lt;product_value&gt;</p>


### 💻 Solution (python):

```python
average = 0
count = 0
total = 0
prod=1
while(True):
  number = input()
  if(number == 'q'):
    break
  count = count + 1
  total = total + float(number)
  prod=prod*float(number)
average = total / count
print("Average is " + str(average))
print("Product of all number is " + str(prod))
```

---

## :question: Question 9 (Order: 9)

<p>Write a program to create a list num of 5  input numbers, then an enter a 6th number to delete it from a created list num, if a 6th number found in the list num otherwise keep a orginal list num and print the resulted list according to the condition.</p>
<p>For example, num=[1,2,3,4,5] and another_num=2 so resulted output list num=[1,3,4,5]</p>


### 💻 Solution (python):

```python
num_list = []
# read five input numbers using for loop
for i in range(5):
  number = input()
  num_list.append(int(number))
  
search = int(input())

for i in range(5):
  if (num_list[i] == search):
    del num_list[i]
    break
print(num_list)
```

---

## :question: Question 10 (Order: 10)

<p>Write a program to create and print a two lists, one containing all even numbers and other containing all odd numbers in the range of 1 to 100.</p>


### 💻 Solution (python):

```python
even = []
odd = []
for i in range(1, 101):
    if (i % 2 == 0):
        even.append(i)
    else:
        odd.append(i)
print(even)
print(odd)

```

---

## :question: Question 11 (Order: 11)

<p>Write a program to create a loop that increments the entered input value by 2 and print the number itself and the incremented values upto an entered limit</p>


### 💻 Solution (python):

```python
number = int(input())
limit = int(input())

print (number)
while True:
    number = number + 2
    if number> limit:
         break
    print (number)

```

---

