# 📚 Questions for ID: 5bb0b39ff1efbf58974404db

## :question: Question 1 (Order: 1)

<p>Write a program to define a two strings in separate lines and print it as a single line.</p>
<p>For example, input string1=“Python is a easy language" and string2= "&amp; high level language.” so output="Python is a easy language &amp; high level language."</p>


### 💻 Solution (python):

```python
string1 = input()
string2 = input()
print (string1 + string2)
```

---

## :question: Question 2 (Order: 2)

<p>Write a program to print the below sentances as below format.</p>
<p>Alice: Hurrah! Only ten days to the holidays.</p>
<p>Bob: I know. I've been counting the days.</p>
<p><strong>Note:</strong> Take spacing between words.</p>


### 💻 Solution (python):

```python
print("Alice: Hurrah! Only ten days to the holidays.\nBob: I know. I\'ve been counting the days.")
```

---

## :question: Question 3 (Order: 3)

<p>Write a program to find the average of an entered three numbers and print the result of it.</p>
<p>For example, input numbers as 15, 23, 25 and output would be a 21.0.</p>


### 💻 Solution (python):

```python
number1 = float(input())
number2 = float(input())
number3 = float(input())
average = (number1 + number2 + number3) / 3
message = "Average is %s"
print(message % average)
```

---

## :question: Question 4 (Order: 4)

<p>Write a program to read an entered first name, lastname and age of a person and print the details in format like "Jonny San is 2 years old."</p>


### 💻 Solution (python):

```python
first_name = input()
last_name = input()
age = input()
print(first_name + " " + last_name + " is " + age + " years old.")
```

---

## :question: Question 5 (Order: 5)

<p>Write a program to create a list of fruits as "Orange, Apple, Mango, Pineapple, Strawberry, Banana" and follow the below instructions to print the output.</p>
<p>1. Print the <strong>n</strong> item in the list of fruits, where <strong>n</strong> is a keyboard input.</p>
<p>2. Print the subset of the list of third to fifth element of fruits.</p>
<p>3. After removing Pineapple and Strawberry from the list<span style="font-family:Courier New,Courier,monospace;">,</span>print the fruit list.</p>


### 💻 Solution (python):

```python
fruits_list = ['Orange', 'Apple', 'Mango', 'Pineapple', 'Strawberry', 'Banana']
n=int(input())
print(fruits_list[n-1])
print(fruits_list[2:5])
del fruits_list[3]
del fruits_list[3]
print(fruits_list)
```

---

## :question: Question 6 (Order: 6)

<p>Write a program to perform following instructions.</p>
<p>1. Create a list of colors having items Green, Yellow, orange, Red, and Pink.</p>
<p>2. Add a new element as new_color to the list of colors, where new_color is a keyboard input.</p>
<p>3. Create another list of numbers 4, 6, 8, 2 and 3.</p>
<p>4. Combine the list of colors and numbers and print the resulted list.</p>


### 💻 Solution (python):

```python
colors = ["Green", "Yellow", "orange", "Red", "Pink"]
# To add a new element
new_color=input()
colors.append(new_color)
# Create a list of numbers
numbers = [4, 6, 8, 2, 3]
# To join two list
print(colors + numbers)


```

---

## :question: Question 7 (Order: 7)

<p>Write a program to perform following instructions for a list num = [6, 7, 3, 8, 1, 5, 16, 13, 11, 19, 2, 4, 12, 9, 17, 10].</p>
<p>1. Print <strong>nth</strong> and 12th element of the list, where <strong>n</strong> is a keyboard input</p>
<p>2. Print the sum of second, third and sixth elements of the list.</p>
<p>3. Create a list sub, which is a sublist of num and contains elements from index position 6 to 13.</p>
<p>4. Create a list new_list by joining num and sub.</p>
<p>5. Replace the second element of new_list with 20.</p>
<p>6. Print the new_list.</p>


### 💻 Solution (python):

```python
num = [6, 7, 3, 8, 1, 5, 16, 13, 11, 19, 2, 4, 12, 9, 17, 10]
n=int(input())
# Print nth and 12th element of the list
print(num[n-1])
print(num[11])
## Print the sum of second, sixth and third elements of the list.
sum_of_three = num[1] + num[2] + num[5]
print(sum_of_three)
# Create a list sub, which is a sublist of num and contains elements from index position 6 to 13.
sub = num[6:14]
# Join num and sub
new_list = num + sub
# Replace the second element of new_list with 20 and print the new_list
new_list[1] = 20
print(new_list)
```

---

## :question: Question 8 (Order: 8)

<p>Write a program which accepts a sequence of comma-separated numbers as an entered input string and generate a list and a tuple which contains every number of entered string.</p>
<p>For example, input string is "12,63,78,16,45,86,23,45" and output would be [12, 63, 78, 16, 45, 86, 23, 45] and (12, 63, 78, 16, 45, 86, 23, 45).</p>
<p><strong>Hint:</strong> Split string values with comma(,)</p>


### 💻 Solution (python):

```python
numstr = input()
list_numstr = numstr.split(",")
print(list_numstr)
print(tuple(list_numstr))
```

---

## :question: Question 9 (Order: 9)

<p>Write a program to perform following instructions.</p>
<p>1. Create a tuple num of numbers from <b>10 to 20</b> including both.<br/>
2. Print <strong>nth</strong> and 8th element of num, where <strong>n </strong>is a keyboard input.<br/>
3. Print the sum of second, third and sixth elements of the tuple.<br/>
4. Create a tuple sub, which is a sublist of num and contains elements from index position 6 to 9.<br/>
5. Join sub and num and print the resulted tuple as new_t.<br/>
 </p>


### 💻 Solution (python):

```python
num = (10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20)
n=int(input())
print(num[n-1])
print(num[7])
print(num[1] + num[2] + num[5])
sub = num[5:10]
new_t = num + sub
print(new_t)
```

---

## :question: Question 10 (Order: 10)

<p>Write a program to perform following instructions for shapes dictionary which corresponding to below table and accepts a Shape Name as a keys and a side as a value.</p>
<table border="1" cellpadding="1" cellspacing="1" style="width: 175px;">
<tbody>
<tr>
<td><strong> Shape Name    </strong></td>
<td><strong> Side    </strong></td>
</tr>
<tr>
<td> Square</td>
<td> 4</td>
</tr>
<tr>
<td> Triangle</td>
<td> 3</td>
</tr>
<tr>
<td> Rectangle</td>
<td> 4</td>
</tr>
<tr>
<td> Pentagon</td>
<td>  5</td>
</tr>
</tbody>
</table>
<p>1) Create a shape dictionary.</p>
<p>2) Print the number of sides of shape_name from the dictionary, where shape_name is a keyboard input.</p>
<p>3) Remove 'Rectangle' key from the dictionary.</p>
<p>4) Alter the value of 'Pentagon' as 6.</p>


### 💻 Solution (python):

```python
# Define a dictionary of shapes
shapes={}
shapes['Square'] = 4
shapes['Triangle'] = 3
shapes['Rectangle'] = 4
shapes['Pentagon'] = 5

# To print the value corresponding to Triangle
shape_name=input()
print(shapes[shape_name])

# To delete Rectangle
del shapes['Rectangle']

# To alter the value of Pentagon
shapes['Pentagon'] = 6
```

---

