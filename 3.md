# 📚 Questions for ID: 5bb0b60df1efbf32a644051a

## :question: Question 1 (Order: 1)

<p><u><strong>Strings</strong></u></p>
<p>In python, strings are collection of letters. It can have any keyboard character and can be as long as we want. String values can be used just like integer or float values. </p>
<p>A string is can be represented by entering a text between two single or double quotation marks. We can store strings in variables like new_string = 'Python is fun !!!'.</p>
<p>The single quotes, tell python where the string begins and ends. They are not part of the string value’s text.</p>
<p><strong>Question</strong>: Write a program to create a variable greeting (where greeting is a keyboard input), which stores the string value and display it.</p>
<p>For example, input string greeting="Morning!" and output is "Morning!".</p>


### 💻 Solution (python):

```python
greeting  = input()
print(greeting)
```

---

## :question: Question 2 (Order: 2)

<p><u><strong>Multiline Strings</strong></u></p>
<p>While creating a string using single quotes (') or double quotes ("), quote must be end on the same line otherwise we will get an error message.</p>
<p>To use more than one line of text in string called a multiline string. It uses three quotes (''') and then hit enter between lines.</p>
<p>For example, multiline_string = '''Python is a high-level <br/>
programming language'''</p>
<p>Another way to create a multiline string is to use '\n' which indicates a new line.</p>
<p>For example, multiline_string = '''Python is a high-level \nprogramming language'''</p>
<p><strong>Question</strong>: Write a program to print following sentance.<br/>
                Salesman: Good evening, sir. How can I help you?<br/>
                Customer: I have come to buy a pair of shoes.<br/>
<strong>Note:</strong> After every punctuation mark ,there is a space except question mark.</p>


### 💻 Solution (python):

```python
# Print statement
print('''Salesman: Good evening, sir. How can I help you?
Customer: I have come to buy a pair of shoes.''')
```

---

## :question: Question 3 (Order: 3)

<p><u><strong>Escape (ignore) Character</strong></u></p>
<p>If the string itself contains a single quote, python may get confused about the quotes inside the string. So use escape character to display the additional quote.</p>
<p>For example, to print sentence as "Don't worry" ,output code should be as "print("Don\'t worry")" where "\" is a escape character.</p>
<p><strong>Question</strong>: Write a program to print "He said: it's over, isn't it?"</p>


### 💻 Solution (python):

```python
print('He said: it\'s over, isn\'t it?')
```

---

## :question: Question 4 (Order: 4)

<p><u><strong>Placeholder text</strong></u></p>
<p>If we want to display a message using the contents of a variable, we can embed values in a string using "%s", which is like a marker for a value that we want to add later. </p>
<p>For example, name is a variable having value "Albert" and we have a message to print "My name is Albert". To get it printed, we can write the code as<br/>
name = "Albert"<br/>
message = "My name is %s"<br/>
print(message % name)</p>
<p><strong>Question</strong>: Write a program to print a message as  "I scored '<strong>N'</strong> points." by using the variable score with value <strong>N</strong> ,where <strong>N</strong> is  a keyboard input.</p>


### 💻 Solution (python):

```python
score = int(input())
message = "I scored %s points."
print(message % score)
```

---

## :question: Question 5 (Order: 5)

<p><u><strong>String Concatenation</strong></u></p>
<p>We can combine string values with operators to make expressions, just as we did with integer and float values. When we combine two strings with the '+' operator, it’s called string concatenation. </p>
<p>For example, print( 'Hello' + 'World!' ) will print HelloWorld. The expression evaluates to a single string value, 'HelloWorld'. There is no space between the words because there was no space in either of the two concatenated strings.</p>
<p>The '+' operator works differently on string and integer values because they are different data types. All values have a data type. The data type of the value 'Hello' is a string. The data type of the value 5 is an integer. The data type tells python what operators should do when evaluating expressions. The '+' operator concatenates string values but adds integer values.</p>
<p><strong>Question</strong>: Write a program to print the single string by joining the two keyboard input words.</p>
<p>For example, input word1="Good " and word2="evening", so output would be Good evening.</p>


### 💻 Solution (python):

```python
word1=input()
word2=input()
print(word1+word2)
```

---

## :question: Question 6 (Order: 6)

<p><u><strong>Repeating a string</strong></u></p>
<p>To repeat a string , we use '*' (asterisk) with string value and number of time to repeat a string</p>
<p>For example, multiply the string "Hello" by 5,we use code as 'Hello' * 5 and output of it would be "HelloHelloHelloHelloHello".</p>
<p>We can multiply a string by 10, just like we multiply the number 5 by 10.</p>
<p>Python programmers might use this approach to line up strings with a specific number of spaces when displaying messages.<br/>
If we assign a string having 20 spaces to a variable, we can use it to specify 20 spaces.</p>
<p><strong>Question</strong>: Write a program to print a string of sequence of <strong>N</strong> asterisk character, where <strong>N</strong> is a keyboard input.</p>


### 💻 Solution (python):

```python
N=int(input())
print("*" * N)
```

---

## :question: Question 7 (Order: 7)

<p><u><strong>Comments</strong></u></p>
<p>Any text following a hash mark (#) is a comment in python. Comments are the programmer’s notes about what the code does; they are not written for python but for the programmer.</p>
<p>Python ignores comments when it runs a program. Programmers usually put a comment at the top of their code to give their program a title. </p>
<p><strong>Question</strong>: Write a program to print the result of the mathematical operation 36 +<strong> 'a'</strong> ,<strong> </strong>where <strong>'a'</strong> is a keyboard input. and add a comment on top of the code to describe the program.</p>


### 💻 Solution (python):

```python
a=int(input())
#This program is used to add two numbers
print(36 + a)
```

---

## :question: Question 8 (Order: 8)

<p><u><strong>Functions</strong></u><br/>
A function is a kind of mini-program inside our program that contains several instructions for python to execute. The great thing about functions is that we only need to know what they do, not how they do it. Python provides some built-in functions like print() function of previous chapters.</p>
<p><strong>Function call:</strong></p>
<p>A function call is an instruction that tells python to run the code inside a function. </p>
<p>For example, our program calls the print() function to display a string on the screen. The print() function takes the string value which type between the parentheses as input and displays that text on the screen.</p>
<p>input() function is another example of built-in function. When the input() is called, the program waits for the user to enter text. The text string, that the user enters becomes the value that the function call evaluates to. Function calls can be used in expressions anywhere a value can be used.</p>
<p>We can assign the value that returned by a function to a variable.<br/>
For example, name = input()</p>
<p>The return value of the input() function is the string that the user entered(like their name). If the user enters Albert, the input() function call evaluates to the string 'Albert' and store it to the variable as name.</p>
<p><strong>Question</strong>: Write a program to read two entered keyboard strings and print the concatenated string of them.</p>


### 💻 Solution (python):

```python
first = input()
second = input()
print(first + second)
```

---

## :question: Question 9 (Order: 9)

<p><u><strong>Type conversion methods</strong></u></p>
<p>Using the int(), float(), and str() functions, we can take a value of one data type and return it as a value of a different data type.</p>
<p>The int() function takes one argument and returns the argument’s value as an integer.<br/>
For example, int ( ' 500 ' ) take the string "500" and return the integer value 500.</p>
<p>we cann't pass any string in it like passing 'five' to int() will result in an error.</p>
<p>The float() and str() functions will similarly return float and string versions of the arguments passed to them.<br/>
For example, when the string '50' or the integer 50 is passed to float(), the float will return 50.0.<br/>
Likewise, when the integer 50 is passed to str(), the string will return '50'. But when the float 50.0 is passed to str(), the string will return '50.0'.</p>
<p><strong>Question</strong>: Write a program to take the name, age and body weight as a keyboard input for two person's details and print the personal information with the average weight of two persons in below output format.</p>
<p>For example, if input is as below table, then output would be as below output format.</p>
<table border="1" cellpadding="1" cellspacing="0" style="width: 300px;">
<thead>
<tr>
<th scope="col">Name</th>
<th scope="col">Age</th>
<th scope="col">Weight</th>
</tr>
</thead>
<tbody>
<tr>
<td>Alice</td>
<td>10</td>
<td>31.5</td>
</tr>
<tr>
<td>Smith</td>
<td>12</td>
<td>34.2</td>
</tr>
</tbody>
</table>
<p><strong>Output Format:</strong></p>
<p>Alice is 10 Years old.</p>
<p>Smith is 12 years old.</p>
<p>Average weight is 32.85.</p>


### 💻 Solution (python):

```python
name1 = input()
age1 = int(input())
weight1 = float(input())
name2 = input()
age2 = int(input())
weight2 = float(input())
average_weight = (weight1 + weight2) / 2
print(name1 + " is " + str(age1) + " years old.")
print(name2 + " is " + str(age2) + " years old.")
print("Average weight is " + str(average_weight)+'.')
```

---

## :question: Question 10 (Order: 10)

<p><u><strong>List</strong></u></p>
<p>Lists are another type of object in python. It is a collection of items like a array. They are used to store a different type of data and an indexed sequence of items.</p>
<p>List values begin with a left square bracket( '[ ') and end with a right square bracket (']'). This is like how strings begin and end with quotation marks.</p>
<p>Commas, separate the individual values inside a list. These values are also called items. Lists store several values without using a variable for each one.</p>
<p>For example, we can create a list of days as</p>
<p>days = ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday']</p>
<p>We are familiar with indexing method used in books to direct us to some particular topic. Each topic has been ordered by it’s page number and we can easily find out the topic we want to reach.</p>
<p>Just like this, List in python are also indexed. Every element in the list is associated with a position number. That is index value.</p>
<p>In python, the index of the first item in a list is 0, the second item is at index 1, the third item is at index 2 and so on. <br/>
In the above example, index value of Sunday is 0, index value of Monday is 1 and so on.</p>
<p><strong>Question</strong>: Write a program to create and print a list animals which containing the elements like Tiger, Lion, Monkey, Elephant and Deer and also print the '<strong>n' </strong>element of list, where '<strong>n'</strong> is a keyboard input and 0-4.</p>


### 💻 Solution (python):

```python
n=int(input())
animals = ['Tiger', 'Lion', 'Monkey', 'Elephant', 'Deer']
print(animals)
print(animals[n])
```

---

## :question: Question 11 (Order: 11)

<p><u><strong>Accessing List Items</strong></u></p>
<p>We can access an item of a list by its index number given between the square brackets([]). We can give forward and backward indexing for list.</p>
<p>For example, list colors = ['red', 'orange', 'yellow', 'blue'] and index value is as below.</p>
<table border="1" cellpadding="1" cellspacing="0" style="width: 400px;">
<thead>
<tr>
<th scope="col"> Forward Indexing</th>
<th scope="col"> 0</th>
<th scope="col"> 1</th>
<th scope="col"> 2</th>
<th scope="col"> 3</th>
</tr>
</thead>
<thead>
<tr>
<th scope="col"> List colors</th>
<th scope="col"> 'red'</th>
<th scope="col"> 'orange'</th>
<th scope="col"> 'yellow'</th>
<th scope="col"> 'blue'</th>
</tr>
</thead>
<thead>
<tr>
<th scope="col"> Backward Indexing</th>
<th scope="col"> -4</th>
<th scope="col"> -3</th>
<th scope="col"> -2</th>
<th scope="col"> -1</th>
</tr>
</thead>
</table>
<p>We can access indexing of list colors by colors[0],colors[1],colors[2] and colors[3] in forward direction and get results accordingy.</p>
<p>For example,colors[0] will return first element of the list colors i.e. red.</p>
<p>We can say python list is a zero indexed because the indexes begin at 0 and not 1. If we try accessing an index that is too high to be in the list, it will result in an error.</p>
<p>We can also access the subset of the list by using a colon (:) inside the square brackets ([ ]). We always includes the first index value, which is given before colon and second last index value which is taken according to last index, which is given after colon.</p>
<p>For example,  In [1:3], 1 is a first index value and 3 is a last index value. [1:3] shows the items from index position 1 up to index position 2 or in other words, items 1 and 2 only. The output syntax is "print(colors[1:3])" and it will print ['orange', 'yellow']. </p>
<p><strong>Question</strong>: Write a program to create a list of months from January to December and print the n, n+1,n+2 months as below output format , where '<strong>n'</strong> is a keyboard input and then print a list, which contains September, October and November.</p>
<p><strong>Output Format:</strong></p>
<p>1. n month</p>
<p>2. n+1 month</p>
<p>3. n+2 month</p>
<p><strong>Note: </strong>A 'n' should be between 0-10.</p>
<p>For example, n=0 so output would be as below.</p>
<p>1. January<br/>
2. February<br/>
3. March<br/>
['September', 'October', 'November']</p>
<p> </p>


### 💻 Solution (python):

```python
months = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
n=int(input())
print('1. ' + months[n]) 
print('2. ' + months[n+1])
print('3. ' + months[n+2])
print(months[8:11])
```

---

## :question: Question 12 (Order: 12)

<p><strong><u>Add Elements to the list</u></strong></p>
<p>The append() method will add the value we pass as an argument to the end of the list.</p>
<p>For example, if we have a list numbers and wants to add 10 in same list, we use syntax as "numbers.append(10)" and it will add a new element 10 to the end of the list numbers.</p>
<p><strong>Question</strong>: Write a program for a given list num of numbers from 1 to 5 and perform following instructions.</p>
<p>1) Print the list elements.</p>
<p>2) Add the numbers n1 and n2 to the same list, where n1 and n2 is a keyboard input.</p>
<p>3) Print the list with new element.</p>


### 💻 Solution (python):

```python
numbers = [1, 2, 3, 4, 5]
print(numbers)
n1=int(input())
n2=int(input())
numbers.append(n1)
numbers.append(n2)
print(numbers)
```

---

## :question: Question 13 (Order: 13)

<p><u><strong>Remove Elements from the list</strong></u></p>
<p>The <span style="font-family:Courier New,Courier,monospace;">del </span>command is used to remove an item from the list,</p>
<p>For example, consider a list months= [ ’January’, ‘February’, ‘March’, ‘April’, ‘May’, ‘June’, ‘July’ ]</p>
<p>To remove ‘March’ from this list, try the command as "del months_list[2]" so new list will look like as</p>
<p>[ ’January’, ‘February’, ‘April’, ‘May’, ‘June’, ‘July’ ]</p>
<p><strong>Question</strong>: Write a program for a given list num of numbers from 1 to 10 and perform following instructions.</p>
<p>1) Print the list elements.</p>
<p>2) Remove the numbers 6 and 8 from this list.</p>
<p>3) Remove the <strong>n </strong>element from this list, where <strong>n</strong> is a keyboard input.</p>
<p>4) Print the list after removing elements.</p>


### 💻 Solution (python):

```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
n=int(input())
print(numbers)
del numbers[n-1]
del numbers[4]
del numbers[5]
print(numbers)
```

---

## :question: Question 14 (Order: 14)

<p><u><strong>List Concatenation</strong></u></p>
<p>We can join several lists into one list using the '+' operator, just as we can do with strings, is called list concatenation. </p>
<p>For example, [1, 2, 3, 4] + ['apples', 'oranges'] will result in the new list as [1, 2, 3, 4, 'apples', 'oranges'].</p>
<p>We can’t add a list value and a string value with the '+' operator.</p>
<p><strong>Question</strong>: Write a program for a given two lists as fruits having an elements like Grape, Pineapple and Apple and vegetables having an elements like Tomato, Potato and Carrot and print the combined list of them and a <strong>nth</strong> element of combined llist , where <strong>n</strong> is a keyboard input.</p>


### 💻 Solution (python):

```python
fruits = ['Grape', 'Pineapple', 'Apple']
vegetables = ['Tomato', 'Potato', 'Carrot']
n=int(input())
print(fruits + vegetables)
print(fruits[n-1])
```

---

## :question: Question 15 (Order: 15)

<p><u><strong>Tuples</strong></u></p>
<p>A Tuple is a collection of python objects which are separated by commas and enclosed with parentheses(). In someways a tuple is similar to a list in terms of indexing and operations, the main difference between a tuple and a list is that a tuple cannot  change once you’ve created it.</p>
<p>For example, numbers = (10, 65, 54, 63, 22, 37, 44)</p>
<p>We can access third element of the tuple by accesing 2nd index of tuple as numbers(2). We can join two tuples as numbers and colors by code as numbers + colors.</p>
<p>If we try to replace the first value in the tuple numbers with the number 48 or append any other value, we get an error message.</p>
<p>We would use a tuple instead of a list because sometimes it is useful to use something that we know can never change. If we create a tuple with two elements inside, it will always have those two elements inside.</p>
<p>In case of input data being supplied as a string of comma separated items, we can generate a list of items by using split() method and then convert this list into tuple by  tuple() method and syntax as tuple(list_name).</p>
<p>For example, if data = "10,12,18,15,42,63,98" so syntax as newdata=data.split(',') and print(newdata) will return ['10', '12', '18', '15', '42', '63', '98'] and then conversion syntax as tuple(newdata) will reurn the tuple ('10', '12', '18', '15', '42', '63', '98').</p>
<p><strong>Question:</strong> Write a program to create a tuple even_numbers having elements as even numbers less than 15 and print this tuple as well as the sum of '<strong>n'th</strong> and fourth element of the tuple, where '<strong>n'</strong> is a keyboard input.</p>


### 💻 Solution (python):

```python
even_numbers = (2, 4, 6, 8, 10, 12, 14)
print(even_numbers)
n=int(input())
print(even_numbers[n-1] + even_numbers[3])
```

---

## :question: Question 16 (Order: 16)

<p><u><strong>Dictionary</strong></u></p>
<p>Dictionary is a book that lists the words of a language and gives their meaning likewise in python, a dictionary is a collection of values like a list. But instead of accessing the items in the dictionary with an integer index, we can access them with a keys.</p>
<p><strong>Syntax of dictionary:</strong></p>
<p>&lt;dictionary-name&gt; ={key1:value1, key2:value2,....}</p>
<p>In dictionary, we use colons to separate each key from its value and items are enclosed in braces ({}).</p>
<p>For example, a dictionary <span style="font-family:Courier New,Courier,monospace;">data </span>can be defined as<br/>
data = {'Apple':'Red', 'Banana':'Yellow', 'Cherry':'Red'}</p>
<p><strong>Question</strong>: Write a program to create a dictionary personal_info<span style="font-family:Courier New,Courier,monospace;"> </span>using the following data and acess the age of person by entering the his/her name as a keyboard input and then print it.</p>
<table border="1" cellpadding="1" cellspacing="1" style="width: 300px;">
<thead>
<tr>
<th scope="col">Name</th>
<th scope="col">Age</th>
</tr>
</thead>
<tbody>
<tr>
<td>Diana</td>
<td>15</td>
</tr>
<tr>
<td>Antony</td>
<td>12</td>
</tr>
<tr>
<td>Joe</td>
<td>16</td>
</tr>
</tbody>
</table>


### 💻 Solution (python):

```python
personal_info = {}
personal_info['Diana']=15
personal_info['Antony']=12
personal_info['Joe']=16
name=input()
print(personal_info[name])

```

---

## :question: Question 17 (Order: 17)

<p><u><strong>Access Dictionary Data</strong></u></p>
<p>The values between the curly brackets are key-value pairs of dictionary. The keys are on the left of the colon and the key’s values are on the right of the colon. We can access the values like items in lists by using the key name.</p>
<p>For example, dictionary data = {'Apple':'Red', 'Banana':'Yellow', 'Cherry':'Red'}, we can access first item of dictionary by syntax as data['Apple']. After executing this syntax, we will get the value corresponding to "Apple" i.e. "Red".</p>
<p>Also data.keys() will print all the keys name and data.values() will print all the values of keys as a list.</p>
<p><strong>Question:</strong> Write a program for a given dictionary months having numbers from 1 to 12 as a keys and January to December as a values respectively and perform the following instruction.</p>
<p>1) Print the value corresponding to the numbers 7, 3, 11 and <strong>n,</strong> where <strong>n</strong> is a keyboard input.<br/>
2) Print the all values of months as a list.</p>


### 💻 Solution (python):

```python
months = {1: 'January', 2: 'February', 3: 'March', 4: 'April', 5: 'May', 6: 'June', 7: 'July', 8: 'August', 9: 'September', 10: 'October', 11: 'November', 12: 'December'}
n=int(input())
print(months[7])
print(months[3])
print(months[11])
print(months[n])
print(list(months.values()))
```

---

## :question: Question 18 (Order: 18)

<p><u><strong>Remove or Reassign values</strong></u></p>
<p>To delete a value of a dictionary, we use its key.</p>
<p>For example, to remove Apple from dictionary data = {'Apple':'Red', 'Banana':'Yellow', 'Cherry':'Red'},we should use syntax as  del data['Apple'] so resulted dictionary would be  {'Banana':'Yellow', 'Cherry':'Red'}.</p>
<p>To replace a value in a dictionay, we also use its key.</p>
<p>For example,<font face="Courier New, Courier, monospace">to</font> replace the color of Cherry from "Red" to "Green" , we should use syntax as data['Cherry'] = "Green".</p>
<p><strong>Question:</strong> Write a program to create a dictionary score_card as below data and perform following instructions.</p>
<table border="1" cellpadding="1" cellspacing="1" style="width: 300px;">
<tbody>
<tr>
<td><strong>Subject</strong></td>
<td><strong>Marks</strong></td>
</tr>
<tr>
<td>Mathematics</td>
<td>68</td>
</tr>
<tr>
<td>Language</td>
<td>78</td>
</tr>
<tr>
<td>Science</td>
<td>72</td>
</tr>
<tr>
<td>Humanities</td>
<td>75</td>
</tr>
</tbody>
</table>
<p>1) Print dictionary score_card.</p>
<p>2) Change the marks of Language to 70.</p>
<p>3) Print changed dictionary score_card. </p>
<p>4) Delete the data associted with marks of Humanities.</p>
<p>5) Print resulted dictionary score_card.</p>


### 💻 Solution (python):

```python
score_card = {}
score_card['Mathematics']=68
score_card['Language']=78
score_card['Science']=72
score_card['Humanities']=75
print(score_card)
score_card['Language']=70
print(score_card)
del score_card['Humanities']
print(score_card)

```

---

