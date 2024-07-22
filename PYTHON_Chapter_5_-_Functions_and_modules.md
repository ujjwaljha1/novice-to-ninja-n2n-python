# 📚 Questions for ID: 5bad2021a2da6b668887810c

## :question: Question 1 (Order: 1)

<p><u><strong>Functions</strong></u></p>
<p><meta charset="utf-8"/></p>
<p dir="ltr">In the programming, function is a sequence of commands, that can be reused together later in a program. Functions run the same code multiple times without having to copy and paste that code over and over again. Instead, we put that code inside a function and call the function whenever we need to. Because we write the code only once in the function, if the function’s code has a mistake, we only have to change it in one place in the program.</p>
<p dir="ltr">We’ve already used a few functions like print(), input(), str() and int(). Our programs have called these functions to execute the code inside them.</p>
<p dir="ltr">A function has three parts: a name, parameters and a body.</p>
<p dir="ltr">The keyword <strong>def </strong>introduces the name of the function, parameter lists are optional and given in the parentheses and a colon (:) follows the closing parenthesis and indicates the start of your functions code suite.</p>
<p dir="ltr">For example, a function to print Hello can be defined as</p>
<p>def print_hello ():</p>
<p>        print(“Hello”)</p>
<p>print_hello ()</p>
<p dir="ltr">When we define a function, we specify the instructions for it to run in the function block. Unless we call the function, the instructions in the<strong> def</strong> block will not execute. Later when we call a function, the code inside the <strong>def </strong>block executes.</p>
<p dir="ltr">In other words, when the execution reaches a <strong>def </strong>statement, it skips down to the first line after the <strong>def</strong> block. But when a function is called, the execution moves inside of the function to the first line of the <strong>def</strong> block.</p>
<p dir="ltr">In the above example, the code "print_hello()" is the function call. Calling this function runs the print(“Hello”) code, which displays the “Hello”.</p>
<p dir="ltr">A function’s<strong> def</strong> statement and <strong>def</strong> block must come before we call the function, just as we must assign a value to a variable before we use that variable. If we put the function call before the function definition, we’ll get an error.</p>
<p dir="ltr">For example,in below code, we called the print_hello() function before function definition,</p>
<p dir="ltr">print_hello ()</p>
<p>def print_hello ():</p>
<p>        print(“Hello”)</p>
<p dir="ltr">Traceback (most recent call last):<br/>
  File "&lt;pyshell#0&gt;", line 1, in &lt;module&gt;<br/>
    print_hello ()<br/>
NameError: name 'print_hello' is not defined</p>
<p><strong>Question</strong>: Define a function to print the poem</p>
<p dir="ltr">Whose woods these are I think I know.</p>
<p dir="ltr">His house is in the village though;</p>
<p dir="ltr">He will not see me stopping here</p>
<p dir="ltr">To watch his woods fill up with snow.</p>


### 💻 Solution (python):

```python
def print_poem():
  print('''Whose woods these are I think I know.
His house is in the village though;
He will not see me stopping here
To watch his woods fill up with snow.''')

print_poem()
```

---

## :question: Question 2 (Order: 2)

<p><u><strong>Function Parameters</strong></u></p>
<p><meta charset="utf-8"/></p>
<p dir="ltr">Now let’s look at function parameters. We can define a function to say Hello to a particular person by passing their name as function parameters.</p>
<p>def print_hello ( name ):</p>
<p>        print(“Hello” + name)</p>
<p>print_hello (“Tina”)</p>
<p dir="ltr">In the above example, function parameter is 'name'. When we call 'print_hello()' with an argument 'Tina' in the parentheses, the argument is assigned to the 'name' parameter and the code 'print(“Hello” + name)'  of the function call has been executed with 'Tina' is  assigned to the name parameter so the output would be “Hello Tina”.</p>
<p dir="ltr"><strong>Question</strong>: Define a function to print sum of two entered numbers, x and y.</p>


### 💻 Solution (python):

```python
x = int(input())
y = int(input())

def addition(number1, number2):
  print(number1 + number2)

addition(x, y)
```

---

## :question: Question 3 (Order: 3)

<p><u><strong>The return statement</strong></u></p>
<p><meta charset="utf-8"/></p>
<p dir="ltr">A function is often used to return a value using a return statement. A return statement appears only inside <strong>def block </strong>where a function is defined.</p>
<p dir="ltr">For example, a function to multiply two numbers with a return statement can be define as</p>
<p>def multiplication ( x, y ):</p>
<p>    product = x * y</p>
<p>    return product</p>
<p>multiplication ( 5, 2 )</p>
<p dir="ltr">Once the return statement executes, the program execution jumps immediately out of the <strong>def block</strong> (just as the break statement makes the execution jump out of a while block). Any code after the return statement will never happen. The program execution can moves back to the function by the function call. The function call itself will evaluate to the function’s return value.</p>
<p><strong>Question</strong>: Define a function that returns the smallest number among entered two numbers.</p>


### 💻 Solution (python):

```python
x = int(input())
y = int(input())
# A function to find smallest of two number
def find_smallest(num1, num2):
  if(num1 < num2):
    return num1
  else:
    return num2
smallest = find_smallest(x, y)
print(smallest)
```

---

## :question: Question 4 (Order: 4)

<p><b><u>Variables and Scope (Local and Global)</u></b></p>
<p>A variable that’s inside the body of a function can’t be used again when the function has finished running. Because it exists only inside the function, this is called a <strong>local scope</strong>.</p>
<p><meta charset="utf-8"/></p>
<p dir="ltr">A local scope is created whenever a function is called. What makes variables in local scopes special is that they are forgotten when the function returns and they will be re-created if the function is called again. The value of a local variable isn’t remembered between function calls.</p>
<p dir="ltr">In the below example, we find the product of two numbers and define function for that,</p>
<p>def multiplication ( x, y ):</p>
<p>    product = x * y</p>
<p>    return product</p>
<p>multiplication ( 5, 2 )</p>
<p dir="ltr">If we try to print the variable 'product'<font face="Courier New, Courier, monospace"> </font>outside the function definition, it will result in an error.</p>
<p dir="ltr">If a variable is defined outside the function, it has a different scope or we can say it has a global scope.</p>
<p dir="ltr">Variables that are assigned and defined outside of the function is called a <strong>global scope</strong>. The global scope is created, when our program begins and destroyed ,when our program terminates.</p>
<p dir="ltr">When a global scope is destroyed, the all variables related to it are forgotten because if it remembered the values of variables ,then when we next time ran our program, the variables would remember their values from the last time we ran it and it will effect our current program.</p>
<p dir="ltr">A variable that exists in a local scope is called a local variable, while a variable that exists in the global scope is called a global variable. A variable must be one or the other; it cannot be both local and global.</p>
<p dir="ltr">Local and global variables can have the same name but they are different variables because they are in different scopes.</p>
<p dir="ltr">For example,</p>
<p>product = 100</p>
<p>def multiplication ( x, y ):</p>
<p>     product = x * y</p>
<p>     return product</p>
<p>multiplication ( 5, 2 )</p>
<p dir="ltr">In the above code, the variable 'product'<span style="font-family:Courier New,Courier,monospace;"> </span>that defined inside and outside the function definition and they are not same.</p>
<p><strong>Question</strong>: Define a two variables with name as 'message' and make it global and local, and then write a program to print one variable value as “This variable is in global scope” and  an another variable value as “This variable is in local scope” according to defined variable values and calling function. The output should be displayed first global variable value then the local variable value.</p>


### 💻 Solution (python):

```python
message = "This variable is in global scope"

def print_message():
  message = "This variable is in local scope"
  print(message)

print(message)
print_message()
```

---

## :question: Question 5 (Order: 5)

<p><u><strong>Modules</strong></u></p>
<p><meta charset="utf-8"/></p>
<p dir="ltr">Python includes many built-in functions, some functions are written in separate programs called modules. We can use these functions by importing their modules into our program with an <strong>import statement</strong>.</p>
<p dir="ltr">For example, time module allows us to use various time related functions like localtime(), sleep() etc.</p>
<p dir="ltr">We can import the module using the statement <strong>import time</strong> and call built-in functions that are available in this module, using the <strong>dot symbol</strong>.</p>
<p dir="ltr">For example,</p>
<p>import time</p>
<p>print(time.asctime())</p>
<p dir="ltr"><span style="font-family:Arial,Helvetica,sans-serif;">the above code will return the current date and time, as a string in specific format.</span></p>
<p dir="ltr"><strong>Question</strong>: Write a program to find a factorial of an entered number by importing module.</p>


### 💻 Solution (python):

```python
import math
x = int(input())
# Find factorial using math module
print(math.factorial(x))

```

---

