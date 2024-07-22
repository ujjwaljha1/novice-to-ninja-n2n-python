# 📚 Questions for ID: 5bb0bbe3f1efbfc5334405fd

## :question: Question 1 (Order: 1)

<p><u><strong>Python Operators</strong></u><br/>
The basic symbols like (+,-,*,/ etc) used to perform mathematical operations are called operators.</p>
<p>Operators tell python what to do with the numbers surrounding them. The plus sign(+) adds numbers, the minus sign (-) subtracts numbers, the asterisk (*) multiplies numbers, and the slash (/) divides numbers. </p>
<p>We can use python shell to perform mathematical calculations like 5 + 6, 6 / 2 etc.</p>
<p>For example, if add two numbers as 300 and 100, the output code would be "print(300 + 100)" and output will be 400. </p>
<p><strong>Note</strong>: Python use print function to display the content.</p>
<p><strong>Question: </strong>Write a program to print the following mathematical operations in different lines.<br/>
1. Add 200 and 300<br/>
2. Divide 250 by 50<br/>
3. Subtract 100 from 500<br/>
4. Product of '<strong>a'</strong> and 50<strong> </strong>,where '<strong>a' </strong>is a keyboard input</p>


### 💻 Solution (python):

```python
a=int(input())
print(200 + 300)
print(250 / 50)
print(500 - 100)
print(a * 50)
```

---

## :question: Question 2 (Order: 2)

<p><u><strong>Evaluating Expressions</strong></u><br/>
Expressions are made up of values (the numbers) connected by operators (the math signs) that produce a new value.</p>
<p>For example, 10 + 30 is an expression where values 10 and 30 are connected by an operator ‘ + ‘.</p>
<p>When a computer solves the expression 10 + 30 and returns the value 40, it has evaluated the expression.</p>
<p>Evaluating an expression reduces the expression to a single value, just like solving a math problem reduces the problem to a single number.</p>
<p>When python evaluates an expression, it has an order of precedence in which these are going to be calculated.</p>
<p>The rules of evaluating an expression are follows.</p>
<ul>
<li>1) Multiplication and division always go before addition and subtraction.</li>
<li>2) We use parentheses to control the order of operations.</li>
<li>3) Parts of the expression inside parentheses are evaluated first.</li>
<li>4) Parentheses can be nested, which means that there can be parentheses inside parentheses.</li>
<li>5) Python evaluates the innermost parentheses first, then the outer ones.</li>
</ul>
<p>For example,an expression 7 + 6 * 2 + 4 evaluates to 23 because 6  * 2 (=12) is evaluated first and then do addition 7+12+4(=23).</p>
<p>An expression (7 + 6) * (2 + 4) evaluates to 78 because the (7 + 6) and (2 + 4) inside parentheses are evaluated before multiplication so (7 + 6)=13 and (2 + 4)=6 and then 13*6=78.</p>
<p><strong>Question</strong>: Write a program to print the result of the following statement.</p>
<p>Add 10 to 8, then Multiply the result by 2, then subtract 11 from the result and divide it by <strong>'a'</strong> where a is a keyboard input.</p>


### 💻 Solution (python):

```python
a=int(input())
print((((10 + 8) * 2) - 11) / a)
```

---

## :question: Question 3 (Order: 3)

<p><u><strong>Variables</strong></u></p>
<p>The word variable in programming, describes a place to store information such as numbers, text, lists of numbers, list of texts etc.<br/>
When an expression evaluates to a value, we can use that value later by storing it in a variable.</p>
<p><strong>Syntax to assign a value to a variable: </strong></p>
<p>&lt;name of variable&gt; = &lt;value&gt; , where "=" is a assignment operator</p>
<p>For example,  price = 500</p>
<p><strong>Question: </strong>Write a program to assign the value '<strong>a' </strong>(where '<strong>a'</strong> is a keyboard input) to the variable 'first', then assign the contents of 'first' to variable 'second' and print the variable 'second'.</p>


### 💻 Solution (python):

```python
a=int(input())
first = a
second = first
print(second)
```

---

## :question: Question 4 (Order: 4)

<p><u><strong>Naming a variable </strong></u><br/>
In python, all variables and functions name are case sensitive means MYVAR is not the same as MyVar nor  myvar. It is possible to have multiple distinct variables with the same name but different casing. </p>
<p><strong>Rules for naming of variable: </strong></p>
<p>1) Variable names can be made up of letters, numbers, and the underscore character ( _).</p>
<p>2) They can’t start with a number. we can use anything from single letters (such as a) to long sentences for variable names.</p>
<p>3) A variable can’t contain a space, so use an underscore to separate words.</p>
<p>4) It is not allowed to use keywords as variable name like print, for, while,if etc. keywords of python not used as a variable name because they are used to do some specific function in python program like loop function, condition function etc.</p>
<p>For examples, someVariable = 10, Total_price = 100</p>
<p><strong>Question:</strong>  For a given gallon value <strong>G</strong>, write a program to calculate and display the car's MPG by assigning a value 100 to the total number of miles he or she has driven and <strong>G</strong> to the gallons of gas used.</p>
<p><strong>Note: </strong>A car’s MPG can be calculated as Car's MPG = miles driven / gallons of gas used</p>


### 💻 Solution (python):

```python
miles_driven = 100
G=int(input())
MPG = miles_driven / G
print(MPG)
```

---

