# 📚 Questions for ID: 5baa72e94813f0db7f497a32

## :question: Question 1 (Order: 1)

<p>Built-in functions are already defined within python to do a particular task. Before writing a program we must be aware of important built-in functions as well as modules so that we will be able to solve complex problems using them.</p>
<p><strong><u>The abs() function</u></strong></p>
<p>Absolute value is the value of a number without its sign. The abs() function returns the absolute value of a number. <br/>
For example, absolute value of 8 is 8 and absolute value of -8 is 8.</p>
<p>We might use the abs() function to do something like calculate an absolute amount of movement of a character in a game. Take positive values if move towards right and negative if move towards left. We can calculate total movements by adding absolute value of movement in each direction.</p>
<p>For example, <br/>
left = -21<br/>
right = 36<br/>
total_movement = abs(left) + right</p>
<p><strong>Question</strong>: Write a program to find the absolute value  of  'r', where r=|z|= square root of (x^2+y^2) and complex number z = x + yj.</p>


### 💻 Solution (python):

```python
import math

x = int(input())
y = int(input())

absolute_value = abs(math.sqrt(x * x + y * y))
print("%0.1f" %absolute_value)

```

---

## :question: Question 2 (Order: 2)

<p><u><strong>The bool() function</strong></u></p>
<p>The name bool is a short for boolean. Programmers use the word boolean to describe a type of data that can have one of two possible values, usually either true or false.</p>
<p>The bool() function takes a single parameter and returns either True or False based on its value. We might use bool when we need to decide whether a value has been set or not.</p>
<pre>
<code class="language-python">if (bool(age)):
    print(“Age is” + str(age))
else:
    print(“Data not available”)</code></pre>
<p>When using bool() function for numbers, 0 returns False and any other number returns True.</p>
<p>For example,<br/>
print(bool(0)) will return False<br/>
print(bool(10)) will return True<br/>
print(bool(-3)) will return True<br/>
print(bool(1.5)) will return True </p>
<p>When we use bool() function for strings, it returns False if there’s no value for the string otherwise, it will return True.</p>
<p>For example,<br/>
print(bool(None)) will return False<br/>
print(bool(“”)) will return False<br/>
print(bool(“ ”)) will return True<br/>
print(bool(“Python”)) will return True</p>
<p>The bool function will return False for lists, tuples and dictionary, when it doesn't contain any values otherwise returns True.</p>
<p>For example,<br/>
my_list = []<br/>
print(bool(my_list)) will return False<br/>
my_tuple = ('a', 'b', 'c')<br/>
print(bool(my_tuple))will return True</p>
<p><strong>Question</strong>:Write a code to find the output of the followings.</p>
<p>i) bool(54.85)<br/>
ii) bool(“live”)<br/>
iii) bool(list(range(0, 3, 4)))</p>


### 💻 Solution (python):

```python
print(bool(54.85))
print(bool("live"))
print(bool(list(range(0, 3, 4))))
```

---

## :question: Question 3 (Order: 3)

<p><u><strong>The exec() function</strong></u></p>
<p>"The exec() function is used for the dynamic execution of program which can either be a string or object code. We can say that exec function is like an eval,only difference is that eval only accepts a single expression and returns a value that we can save in a variable and exec accepts a large blocks of code and doesn't return a value."</p>
<pre>
<code class="language-python">my_program = '''print(‘Hello') 
         print(‘World')''' 
exec(my_program)

Output:
Hello
World</code></pre>
<p><br/>
In the above code,the first two lines used to create a variable with a multiline string containing two print statements and then use exec() function to run the string variable. So output shows 'Hello World'.</p>
<p><strong>Question</strong>: Write a code to find the output of the 'a = 10\nb=15\nprint("Sum =", a+b)'   ,using exec() function.</p>


### 💻 Solution (python):

```python
program = 'a = 10\nb=15\nprint("Sum = "+ str(a + b))'
exec(program)
```

---

## :question: Question 4 (Order: 4)

<p><u><strong>The len() function</strong></u></p>
<p>The len() function returns the number of items in an object.</p>
<p>When the object is a string, the len() function returns the number of characters in the string.</p>
<p>For example, len('this is a test string')  will return 21</p>
<p>print(len(['pen', 'book', 'ball'])) will return 3</p>
<p>print(len({'Circle': 'Red', 'Square': 'Blue', 'Triangle': 'Green'})) will return 3</p>
<p><strong>Question</strong>: Write a code to find the length of the list of numbers from 25 to 63 and print the result.</p>


### 💻 Solution (python):

```python
numbers = list(range(25, 64))
print(len(numbers))
```

---

## :question: Question 5 (Order: 5)

<p><u><strong>The min() and max() function</strong></u></p>
<p>The max() function returns the largest item in a list, tuple or string.<br/>
The min() function returns the smallest item in the list, tuple or string. </p>
<p><strong>Note:</strong> Letters are ranked alphabetically and lowercase letters come after uppercase letters in ranked Eg. z &gt; A. </p>
<p>We can call the max() function directly and enter the items that we want to compare into the parentheses as parameters.</p>
<p>For example,  numbers = [15, 40, 10, 35, 11] and output as max=40 and min = 10 by using below code.</p>
<pre>
<code class="language-python">numbers = [15, 40, 10, 35, 11] 
print(max(numbers))# for max value
print(min(numbers))# for min value</code></pre>
<p>We can also use a string with the characters separated by commas or spaces for max() function as below.</p>
<pre>
<code class="language-python">strings = ‘a,b,w,v,f,b,z,A,Y,H,M, ‘ 
print(max(strings)) # for max value

Output:
Z</code></pre>
<p><strong>Question</strong>:Write a code to find the smallest and the largest numbers in the list as [12, 78, 5, 46, 32, 52, 61, 43] and print the result.</p>


### 💻 Solution (python):

```python
numbers=[12, 78, 5, 46, 32, 52, 61, 43]
print(min(numbers))
print(max(numbers))
```

---

## :question: Question 6 (Order: 6)

<p><strong><u>The range() function</u></strong></p>
<p>The range() function is mainly used in for loops, to loop through a section of code a specific number of times. The first two parameters given to range are called the start and the stop range. The numbers that range() function generates begin with the number given as the first parameter and end with the number that’s one less than the second parameter. </p>
<p>The range() function actually returns a special object called an iterator that repeats an action a number of times.We can convert the iterator into a list by using the function list().</p>
<p>For example, print(list(range(0, 50))) will print a list of numbers from 0 to 49.</p>
<p>We can also add a third parameter to range() function called step. If the step value is not included, the number 1 is used as the step by default. </p>
<p>For example, count_by_twos = list(range(0, 30, 2)), where each number in the list increases by two from the previous number.</p>
<p>We can also use negative steps as below.<br/>
count_down_by_twos = list(range(40, 10, -2),where each number in the list decreases by two from the previous number.</p>
<p><strong>Question</strong>: Write a code to print all the numbers which are multiple of 5 in the range of 500 to 550.</p>


### 💻 Solution (python):

```python
print(list(range(500, 551, 5)))

```

---

## :question: Question 7 (Order: 7)

<p><u><strong>The sum() Function</strong></u></p>
<p>The sum() function adds each item of a list and returns the total of them. <br/>
For example, input list numbers = [10, 20, 30, 40, 50, 60, 70] and after executing the below code, sum of all elements of list is 280.</p>
<pre>
<code class="language-python">numbers = [10, 20, 30, 40, 50, 60, 70]
print(sum(numbers))</code></pre>
<p><strong>Question</strong>: Write a code to find the sum of the numbers from 44 to 66 and print the result of sum.</p>


### 💻 Solution (python):

```python
print(sum(list(range(44, 67)))) 

```

---

## :question: Question 8 (Order: 8)

<p><u><strong>The dir() function</strong></u></p>
<p>The dir() function (short for directory) returns the information about any value.  Basically, it tells us the functions that can be used with that value in alphabetical order in a list.</p>
<p>For example, to display the functions, that are available for a list value [“1”, “P”, “M”], write a code as below.</p>
<p>dir([“1”, “P”, “M”])</p>
<p>The dir() function works on anything, including strings, numbers, functions, modules, objects, and classes.</p>
<p><strong>Question: </strong>Write a code for dir () function on an integer value 2 and print the result.</p>


### 💻 Solution (python):

```python
print(dir(2))

```

---

## :question: Question 9 (Order: 9)

<p><u><strong>Working with files</strong></u></p>
<p>Python’s built-in open() function opens a file in the python shell and displays its contents.</p>
<p>The code of opening a file is as below.</p>
<pre>
<code class="language-python">test_file = open(Enter your file location) 
text = test_file.read()
print(text)</code></pre>
<p><strong>Question</strong>: If created a python file as 'code.py' in home folder, then how can print the content of the file 'code.py' using python?</p>


### 💻 Solution (java):

```java

```

### 📝 Answer Options:

1. ❌ 
<p>test_file = open("\home\code.py") <br/>
text = file.read(test_file)<br/>
print(text)</p>


2. ❌ 
<p>test_file = open(\home\code.py) <br/>
text = file.read(test_file)<br/>
print(text)</p>


3. ❌ 
<p>test_file = open(\home\code.py) <br/>
text = test_file.read()<br/>
print(test_file)</p>


4. ✅ **Correct Answer:**
<p>test_file = open("\home\code.py") <br/>
text = test_file.read()<br/>
print(text)</p>


---

## :question: Question 10 (Order: 10)

<p><u><strong>Writing on files</strong></u></p>
<p>We use below steps to write anything into the file.</p>
<p>First we need a file to write so we create a file by using below code.</p>
<p>test_file = open('c:\\myfile.txt', 'w')</p>
<p>When we call test_file,it creates a new and empty file in writing mode denoted by string 'w' means the parameter 'w' tells python that we want to write to the file object, rather than read from it.</p>
<p>To add information to this new file ,we need a write() function as below.<br/>
    test_file.write('this is my test file'), where 'this is my test file' is a string which we want to write in a file.</p>
<p>Finally, we need to tell python when we’re finished writing to the file, using the close function:<br/>
    test_file.close()</p>
<p><strong>Question:</strong> Which of the following code will write "Test" in code.py file?</p>


### 💻 Solution (java):

```java

```

### 📝 Answer Options:

1. ❌ 
<p>test_file = open("code.py", "w")<br/>
test_file.write('Test')</p>
<p>test_file.close()<br/>
text = test_file.read()</p>
<p>print(text)</p>


2. ✅ **Correct Answer:**
<p>test_file = open("code.py", "w")<br/>
test_file.write('Test')</p>
<p>test_file.close()</p>
<p>test_file = open("code.py")<br/>
text = test_file.read()</p>
<p>print(text)</p>


3. ❌ 
<p>test_file.write('Test')</p>
<p>test_file.close()</p>
<p>test_file = open("code.py")<br/>
text = test_file.read()</p>
<p>print(text)</p>


4. ❌ 
<p>test_file = open("code.py", "w")<br/>
test_file.write('Test')</p>
<p>test_file.close()</p>
<p>text = test_file.read()</p>
<p>test_file = open("code.py")</p>


---

