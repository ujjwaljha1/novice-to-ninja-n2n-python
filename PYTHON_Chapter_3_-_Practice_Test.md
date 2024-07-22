# 📚 Questions for ID: 5bb0b846f1efbfe0d644058c

## :question: Question 1 (Order: 1)

<p>Write a program to read a number from user and print "You have reached the maximum limit" if the number is greater than 60 else print "You are under limit".</p>


### 💻 Solution (python):

```python
user_input = int(input())
# if-else statement
if (user_input > 60):
  print("You have reached the maximum limit")
else:
  print("You are under limit")
```

---

## :question: Question 2 (Order: 2)

<p>Write a program to read an entered value as an amount of money and if the amount is greater than 1000, the program should display "You are rich" otherwise print "You are not rich".</p>


### 💻 Solution (python):

```python
money = input()
if int(money) > 1000:        
  print("You are rich") 
else:
  print("You are not rich") 
```

---

## :question: Question 3 (Order: 3)

<p>Write a program to find the greatest number among the two numbers ( x and y) without using else option.</p>


### 💻 Solution (python):

```python
x = int(input())
y = int(input())
# if statement
if(x > y):
  print(x)
# if statement
if(y > x):
  print(y)
```

---

## :question: Question 4 (Order: 4)

<p>Write a program to find the greatest of two numbers (x and y) by using else option</p>


### 💻 Solution (python):

```python
x = int(input())
y = int(input())
# if-else statement
if(x > y):
  print(x)
else:
  print(y)
```

---

## :question: Question 5 (Order: 5)

<p>Write a program to check whether an entered number is less than 10 or greater than 70 and print the message “Too few or Too many” if the condition is true.<br/>
 </p>


### 💻 Solution (python):

```python
user_input = int(input())
# Check user input
if(user_input > 70):
  print("Too many")
elif(user_input < 10):
  print("Too few")

```

---

## :question: Question 6 (Order: 6)

<p>Write a program to check whether the amount of money, which is contained in the variable 'money' is between 100 and 500 ( both numbers are inclusive ) or between 1,000 and 5,000 ( both numbers are inclusive ) and print "Yes" if condition is satisfied otherwise print "No".</p>


### 💻 Solution (python):

```python
money = int(input())
# Check the condition
if((money >= 100 and money <= 500) or (money >= 1000 and money <= 5000)):
    print("Yes")
else:
    print("No")
```

---

## :question: Question 7 (Order: 7)

<p>Write a program to read an input value as a marks and prints "Above average" ,if an entered input is between 50 and 60 (both numbers are not included).</p>


### 💻 Solution (python):

```python
marks = int(input())
# if statements
if (50 < marks < 60):
  print("Above average")
```

---

## :question: Question 8 (Order: 8)

<p>Write a program to read an entered input value and print "Out of range" ,if the entered value is less than zero or print "Proceed", if the entered value is greater than 100.</p>


### 💻 Solution (python):

```python
user_input = int(input())
if(user_input < 0 or user_input > 100):
  print("Out of range")
else:
  print("Proceed")
```

---

## :question: Question 9 (Order: 9)

<p>Write a program to check whether a candidate is eligible or not based on the below conditions and print messag as 'Eligible' , if a below conditions are satisfied otherwise print 'Not Eligible'.</p>
<p>Eligible conditions for an admission of a student to a high school course :<br/>
      1.  Marks in mathematics greater than or equal to 60<br/>
      2.  Marks in science greater than or equal to 50<br/>
      3.  Marks in language is greater than or equal to 40<br/>
      OR<br/>
      Total marks in mathematics and science is greater than or equal to 150</p>
<p><strong>Note</strong>: User input marks sequence as a mathematics, science and language </p>


### 💻 Solution (python):

```python
math = int(input())
science = int(input())
language = int(input())
if ((math >= 60 and  science >= 50 and language >= 40) or math + science >= 150):
    print("Eligible")
else:
    print("Not Eligible")
```

---

## :question: Question 10 (Order: 10)

<p>Write a program to check if a character is a vowel or consonant.</p>
<p><strong>Note</strong>:An entered character should be in lower case.</p>


### 💻 Solution (python):

```python
char = input()
if (char == "a" or  char == "e" or char == "i" or char == "o" or char == "u"): 
    print("Vowel")
else:
    print("Consonant")
```

---

## :question: Question 11 (Order: 11)

<p>Write a program to print the number of days of an entered month.</p>


### 💻 Solution (python):

```python
month = input()
if (month == "January" or month == "March" or month == "May" or month == "July" or month == "August" or month == "October" or month == "December" ): 
    print("31 Days")
elif (month == "April" or month == "June" or month == "September" or month == "November" ):
    print("30 Days")
elif (month == "February" ):
    print("28 or 29 Days")
else:
    print("Invalid Month")
```

---

## :question: Question 12 (Order: 12)

<p>Write a program to read the denomination value of a banknote from the user and display the name of the individual entry,which appears on the banknote of the entered amount, if entry exist in the below list otherwise print 'Invalid Entry'.</p>
<table align="left" border="1" cellpadding="1" cellspacing="1" style="width: 400px;">
<tbody>
<tr>
<td><strong>Individual Entry  </strong></td>
<td><strong>Denomination value of a banknote</strong></td>
</tr>
<tr>
<td>George Washington</td>
<td>$1</td>
</tr>
<tr>
<td>Thomas Jefferson </td>
<td>$2</td>
</tr>
<tr>
<td>Abraham Lincoln</td>
<td>$5</td>
</tr>
<tr>
<td>Alexander Hamilton</td>
<td>$10</td>
</tr>
<tr>
<td>Andrew Jackson</td>
<td>$20</td>
</tr>
<tr>
<td>Ulysses S. Grant </td>
<td>$50</td>
</tr>
<tr>
<td>Benjamin Franklin</td>
<td>$100</td>
</tr>
</tbody>
</table>
<p> </p>


### 💻 Solution (python):

```python
denom = int(input())
if (denom == 1): 
    print("George Washington")
elif (denom == 2): 
    print("Thomas Jefferson")
elif (denom == 5): 
    print("Abraham Lincoln")
elif (denom == 10): 
    print("Alexander Hamilton")
elif (denom == 20): 
    print("Andrew Jackson")
elif (denom == 50): 
    print("Ulysses S. Grant")
elif (denom == 100): 
    print("Benjamin Franklin")
else:
    print("Invalid Entry")
```

---

## :question: Question 13 (Order: 13)

<p>Write a program to read a month name and day(1-31) from the user input and print the season name from the below table against the entered month-day value, which exist in below table month-day range.  The output should be shown as '&lt;season_name&gt; Season' like Spring Season for spring result.</p>
<p><strong>Note: </strong>In below table, take a range of month and day for every season like for a sprimng season consider range as March 20 to June 20.</p>
<table border="1" cellpadding="1" cellspacing="1" style="width: 300px;">
<thead>
<tr>
<th scope="col">Season</th>
<th scope="col">First day</th>
</tr>
</thead>
<tbody>
<tr>
<td>Spring</td>
<td>March 20</td>
</tr>
<tr>
<td>Summer</td>
<td>June 21</td>
</tr>
<tr>
<td>Fall</td>
<td>September 22</td>
</tr>
<tr>
<td>Winter</td>
<td>December 21</td>
</tr>
</tbody>
</table>
<p> </p>


### 💻 Solution (python):

```python
month = input()
day = int(input())

if (((month == 'March') and (day >= 20 and day <= 31)) or((month == 'April' or month == 'May') and (day >= 1 and (day <= 31 or day<=30))) or ((month == 'June') and (day >= 1 and day <= 20))):
    print("Spring Season")

elif (((month == 'June') and (day >= 21 and day <= 30)) or((month == 'July' or month == 'August') and (day >= 1 and (day <= 31 or day<=30))) or ((month == 'September') and (day >= 1 and day <= 21))):
    print("Summer Season")

elif (((month == 'September') and (day >= 22 and day <= 30)) or((month == 'October' or month == 'November') and (day >= 1 and (day <= 31 or day<=30))) or ((month == 'December') and (day >= 1 and day <= 20))):
    print("Fall Season")

elif (((month == 'December') and (day >= 21 and day <= 31)) or((month == 'January' or month == 'February') and (day >= 1 and (day <= 31 or day<=30))) or ((month == 'March') and (day >= 1 and day <= 19))):
    print("Winter Season")
```

---

## :question: Question 14 (Order: 14)

<p>Write a program to read an week number and print the week day against the entered week number.</p>


### 💻 Solution (python):

```python
week_num = int(input())

if (week_num == 1):
    print("Sunday")
elif (week_num == 2):
    print("Monday")
elif (week_num == 3):
    print("Tuesday")
elif (week_num == 4):
    print("Wednesday")
elif (week_num == 5):
    print("Thursday")
elif (week_num == 6):
    print("Friday")
elif (week_num == 7):
    print("Saturday")
else:
    print("Invalid")
```

---

## :question: Question 15 (Order: 15)

<p>Write a program to check an entered length and breadth is for a square or not and print 'Square', if it is for square otherwise print 'Rectangle'.</p>
<p><strong>Note</strong>: User input sequence as a length and breadth. </p>


### 💻 Solution (python):

```python
length = int(input())
breadth = int(input())
if (length == breadth):
  print ("Square")
else:
  print ("Rectangle")
```

---

## :question: Question 16 (Order: 16)

<p>Write a program to take a 3 inputs as an age of 3 people and determine the youngest among them. The output format should be required as 'Youngest age is 5', if age=5 is smaller than others.</p>


### 💻 Solution (python):

```python
first_person = int(input())
second_person = int(input())
third_person = int(input())
message = "Youngest age is %s"
if (first_person < second_person and first_person < third_person):
  print (message % first_person)
elif (second_person < first_person and second_person < third_person):
  print (message % second_person)
elif (third_person < first_person and third_person < second_person):
  print (message % third_person)
```

---

