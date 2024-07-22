# 📚 Questions for ID: 5bb0a9b9f1efbf737644046c

## :question: Question 1 (Order: 1)

<p><u><strong>IF Statements</strong></u></p>
<p>The program execution started at the top instruction in the program and moved straight down and executing each instruction in order. But with some statements, we can control the flow of the program based on conditions. These kinds of statements are called flow control statements. Since they change the flow of the program execution as it moves around our program. Flow control statements includes conditional statements and loops.</p>
<p>In day to day life, we make decisions based on our situation and each our decision will have a certain effect on what we ended up doing. Every decision we make can be modeled as a series of true and false statements.</p>
<p>In programming also, we often ask yes or no questions and decide to do something based on the answer. These sorts of questions are called <strong>conditions</strong>.</p>
<p><strong>Conditional statements </strong>are the digital equivalent of the decisions we make, where our code does something different depending on whether something is <strong>true </strong>or <strong>false</strong>. </p>
<p>For example, in a situation where we need to do something only if some conditions are True, we can use if statements.</p>
<p>Structure of if statement is, the word if, followed by a condition and colon. On next line, write commands to be run.</p>
<pre>
<code class="language-python">if(marks == 50):
      print("Good")</code></pre>
<p>The if statement will run, if the if statement’s condition evaluates to True and if the condition is False, the code in the if block is skipped. Using if statements, we can make the program run certain code only when we want it to.</p>
<p><strong>Question</strong>: Write a program to print a message "Invalid" if an entered number is less than zero otherwise print number.</p>


### 💻 Solution (python):

```python
num = int(input())
if(num < 0):
  	print("Invalid")
if(num > 0):
  print(num)
```

---

## :question: Question 2 (Order: 2)

<p><u><strong>Block of Statements</strong></u></p>
<p>Several lines of code can be grouped together in a block. Every line in a block of code begins with at least the number of spaces as the first line in the block. We can tell where a block begins and ends by looking at the number of spaces at the front of the lines. This is the line’s indentation.</p>
<p>For example, if we want to execute more than one commands  and if a certain condition is true, we can group the commands together by applying equal number of spaces before the command is going to be started. See below code.</p>
<pre>
<code class="language-python">if(number == 0):
    print("Not valid")
    print("Number must be greater than zero")
    print("Try another")</code></pre>
<p>Python programmers typically use four additional spaces of indentation to begin a block. Any following line that’s indented by that same amount is part of the block. The block ends when there’s a line of code with the same indentation as before the new block started. There can also be blocks within other blocks. </p>
<p><strong>Question</strong>: Write a program to read a number entered by the user ( which is 4 or 5) and prints the previous number of it in separate lines. If number is not equal to user input, then don't print anything. </p>
<p>For example, if input number is 5 then output is 1, 2, 3 and 4 in separate lines and if number is not equal to user input 5, then don't print anything.</p>


### 💻 Solution (python):

```python
num = int(input())
if(num == 5):
  print(1)
  print(2)
  print(3)
  print(4)

if(num == 4):
  print(1)
  print(2)
  print(3)
```

---

## :question: Question 3 (Order: 3)

<p><u><strong>Comparison Operators</strong></u></p>
<p>Before start comparision operator , lets take a view on boolean data type. The boolean data type has only two values as True or False. The boolean values must be entered with an uppercase T or F and the rest of the value’s name in lowercase.</p>
<p>Boolean values can be stored in variables just like the other data types:</p>
<p>isValid = True</p>
<p>We use different symbols in python to create our conditions such as equal to, greater than, less than etc.</p>
<p>When we use comparison operator as below table, the program compares the things and tells us whether the criteria set by the comparison are either True (yes) or False (no).</p>
<p style="margin:0in 0in 10pt"><span style="font-size:11pt"><span style="line-height:normal"><span style="font-family:Calibri,sans-serif"><b><span style="font-size:12.0pt"><span style='font-family:"Times New Roman","serif"'>Comparison operators are:</span></span></b></span></span></span></p>
<table border="1" cellpadding="1" cellspacing="1" style="width: 300px;">
<thead>
<tr>
<th scope="col">Operator</th>
<th scope="col">Operation</th>
</tr>
</thead>
<tbody>
<tr>
<td>&lt;</td>
<td>Less than</td>
</tr>
<tr>
<td>&lt;=</td>
<td>Less than or equal to</td>
</tr>
<tr>
<td>&gt;</td>
<td>Greater than</td>
</tr>
<tr>
<td>&gt;=</td>
<td>Greater than or equal to</td>
</tr>
<tr>
<td>==</td>
<td>Equal to</td>
</tr>
<tr>
<td>!=</td>
<td>Not equal to</td>
</tr>
</tbody>
</table>
<p style="margin:0in 0in 10pt"> </p>
<p>For example, the condition age &gt; 15 asks, “Is the value stored in age greater than 15?” If so, then the condition evaluates to True. If not, the condition evaluates to False.</p>
<p>Be careful not to confuse the assignment operator '=' and the equal to comparison operator, ==. The equal sign '=' is used in assignment statements to store a value to a variable whereas the double equal sign' ==' is used in expressions to see whether two values are equal. It’s easy to accidentally use one when we mean to use the other.</p>
<p>It might help to remember that both the equal to (comparison operator as ==) and the not equal to (comparison operatoras  !=) have two characters.</p>
<p><strong>Question:</strong> Write a program to perform following statements for an entered number.</p>
<p>          1) Print "Positive" if the value is greater than 0.</p>
<p>          2) Print "Negative" if the value is less than 0.</p>
<p>          3) Print "Zero" if the value is equal to 0.</p>


### 💻 Solution (python):

```python
num = int(input())
# if statement to check if the number is positive
if(num > 0):
  print("Positive")
# if statement to check if the number is negative
if(num < 0):
  print("Negative")
# if statement to check if the number is zero
if(num == 0):
  print("Zero")
```

---

## :question: Question 4 (Order: 4)

<p><u><strong>IF-ELSE Statements</strong></u></p>
<p>Else statement means we use if statements to do something, when a condition is not true. We can think of "if-else" statements as saying, "If something is true, then do this or else, do something different".</p>
<p>For example, if-else conditions are written as below for limit value 10.</p>
<pre>
<code class="language-python">if(limit &gt;= 10):
    print("You have reached your limit")
else:
    print("Go to next")</code></pre>
<p>As above, if the limit variable is greater than or equal to the value 10, then the if statement’s condition is True and the if block tells the user that they reached the limit. However, if this condition is False means limit variable is less than 10, then python tries the block of else statement and print the string as 'Go to next'.</p>
<p><strong>Question</strong>: Write a program to print the student's result message as "You are qualified", if the entered total marks is greater than 120 otherwise print the student's result message as  "Not qualified".</p>
<p> </p>


### 💻 Solution (python):

```python
total_marks = int(input())
# Check whether qualified or not
if(total_marks > 120):
  print("You are qualified")
else:
  print("Not qualified")
```

---

## :question: Question 5 (Order: 5)

<p><u><strong>Combining Conditions</strong></u></p>
<p>We can combine two or more conditions by using the keywords '<strong>and' </strong>and <strong>'or'</strong>, which produces shorter and simpler code.</p>
<p>Suppose if input numbers are from 1 to 20 and we need to write a program that checks one of the number is a multiple of 5 or not. As we know 5, 10, 15 and 20 are multiple of 5 but we don't need to check condition for these numbers separately so we can write the code as below.</p>
<pre>
<code class="language-python">if(number == 5 or number == 10 or number == 15 or number == 20):
    print("Multiple of 5")
else: 
    print("Not a multiple of 5")</code></pre>
<p>In above code, the result of two operations combined by <strong>'or'</strong> keyword and it will be true, if any of the condition is satisfied. See below.</p>
<p>True <strong>or</strong> True = True<br/>
False <strong>or</strong> False = False<br/>
True <strong>or</strong> False = True<br/>
False <strong>or</strong> True = True</p>
<p>In the above code, the result of two operations combined by <strong>'and'</strong> keyword and it will be true, only if both conditions are satisfied.</p>
<p>True <strong>and</strong> True = True<br/>
False <strong>and</strong> False = False<br/>
True <strong>and</strong> False = False<br/>
False <strong>and</strong> True = False</p>
<p><strong>Question</strong>: Write a program to print "It's a holiday" if the day enter by the user is Sunday or Saturday otherwise print "Not a holiday".</p>


### 💻 Solution (python):

```python
Weekday = input()
# Check whether the entered day is a holiday or not
if(Weekday =="Sunday" or Weekday =="Saturday"):
  print("It's a holiday")
else:
  print("Not a holiday")
```

---

## :question: Question 6 (Order: 6)

<p><u><strong>ELIF Statements</strong></u></p>
<p>Now we can expand our if-else statement further with elif (short word for else if) statements. We can think of elif or “else-if” statements as saying, “If this is true, do this Or else if this next condition is true, do that Or else if none of them is true, do this last thing.” Instead of making two decisions, we can now compare more than two situations by using elif in between if and else statements.</p>
<p>For example, compare entered number is positive or negative or zero by below code.</p>
<pre>
<code class="language-python">if(number &gt; 0):
    print("Positive")
elif(number == 0):
    print("Zero")
else:
    print("Negative")</code></pre>
<p>In the above code, if the number variable is greater than 0, then the if condition is True and the if block tells the user that the number is positive. However, if this condition is False, then python tries the elif condition next. If number is equal to 0, then the string 'Zero' is printed to the screen. If both conditions are False means number variable is less than 0, then the code tells the user that the number is negative.</p>
<p>We can have as many elif statements as we want. We can also leave off the else block if we don’t need one and just have if-elif statements.</p>
<p><strong>Question: </strong>Write a program to describes the overall perfomance of a student in the exam, based on the following data and an entered total marks of student.</p>
<table border="1" cellpadding="1" cellspacing="1" style="width: 300px;">
<thead>
<tr>
<th scope="col">Marks Criteria</th>
<th scope="col">Message</th>
</tr>
</thead>
<tbody>
<tr>
<td>Greater than 80</td>
<td>Outstanding</td>
</tr>
<tr>
<td>between 61 to 80  </td>
<td>Excellent</td>
</tr>
<tr>
<td>Between 41 to 60 </td>
<td>Good</td>
</tr>
<tr>
<td>Less than or equal to 40       </td>
<td>Not qualified</td>
</tr>
</tbody>
</table>
<p> </p>


### 💻 Solution (python):

```python
total_marks = int(input())
# Give perfomance status using elif
if(total_marks > 80):
  print("Outstanding")
elif(total_marks > 60):
  print("Excellent")
elif(total_marks > 40):
  print("Good")
else:
  print("Not qualified")
```

---

## :question: Question 7 (Order: 7)

<p><u><strong>None - variable with no value</strong></u></p>
<p>In python, we can assign nothing or an empty value to a variable by None. It is the absence of value.</p>
<p>For example, variable name = None and print(name) command display None.</p>
<p><strong>Question:</strong> Write a program to store an entered number into a variable num and set num variable as empty, if an entered value is negative otherwise don't change the variable num value and the output display the stored value of num variable according to conditions.</p>


### 💻 Solution (python):

```python
num = int(input())
if(num < 0):
  num = None
print(num)
```

---

