# 📚 Questions for ID: 5bae17d310cab9591c177876

## :question: Question 1 (Order: 1)

<p><u><strong>The for loop</strong></u></p>
<p>In programming, loops execute a portion of code over and over again until a particular task is complete. Think of the <strong>for statement </strong>as saying, "Execute the code in the following block a certain number of times."</p>
<p>To print numbers from 1 to 100, we don't need to write print command 100 times, instead of it , we can create a single <strong>for loop </strong>which executes 100 times and in each execution it will print numbers from 1 to 100 one by one.</p>
<p>A <strong>for statement</strong> begins with the<strong> for keyword</strong>, followed by a "new variable name", then use "<strong>in"</strong> keyword, then followed "<strong>range()" </strong>function that specifies that how many number of times loops will execute and at last a <strong>colon(:)</strong>. </p>
<p>For example, to print a string "Summer" for 5 times,the code would be as below.</p>
<pre>
<code class="language-python">for i in range(5):
    print("Summer")</code></pre>
<p>In the above code , when python program reaches to the <strong>for statement, </strong>the <strong>for loop</strong> starts to execute the code of block. After running all the code of block, the execution moves back to the top of the block ( i.e at <strong>for statement</strong> ) to run the code of block again. This process is repeated upto 5 times because given range is 5 and each time the execution goes through the loop is called an <strong>iteration.</strong></p>
<p>To set a strat point in range, we have to use the range function as range(start, end + 1).</p>
<p>For example, to print numbers from 1 to 100, range function would be like range(1, 101).</p>
<p><strong>Question</strong>: Write a program to print the numbers from 20 to 30.</p>


### 💻 Solution (python):

```python
for i in range(20, 31):
  print(i)
```

---

## :question: Question 2 (Order: 2)

<p><u><strong>Looping with List Items</strong></u></p>
<p>We can use looping on elements of list as below without using range function.</p>
<p><strong>Syntax:</strong></p>
<p>for items in &lt;variable_name&gt; : , where &lt;variable_name&gt; contains the items/elements of list</p>
<p>For example, we have a list of four friends includes James, Monica, Adam and Rachel. <br/>
i.e. friends_list = ['James', 'Monica', 'Adam', 'Rachel']</p>
<p>We can use for loop as below to say 'Hello' to friends.</p>
<pre>
<code class="language-python">for item in friends:
    print(‘Hello %s' % item)</code></pre>
<p>In the above code, for each item of the friends_list ,store the value in the variable 'item' and then print "Hello" with the contents of that variable like Hello James,Hello Monica .....and so on.</p>
<p><strong>Question</strong>: Write a program to print all the elements of a given list colors, which includes Red, Green, Blue, Black and Yellow.</p>


### 💻 Solution (python):

```python
colors = ['Red', 'Green', 'Blue', 'Black', 'Yellow']
for item in colors:
  print(item)
```

---

## :question: Question 3 (Order: 3)

<p><u><strong>The Break Statement</strong></u><br/>
A break statement tells the execution to jump immediately out of the '<strong>for'</strong> block to the first line after the end of the '<strong>for'</strong> block. The break statement is found only inside loops, such as in a '<strong>for' </strong>block.</p>
<p><meta charset="utf-8"/></p>
<p dir="ltr">For example, suppose we have a random list of two digit numbers and if we need to check whether the number 44 is there in the list, then we have to compare each number of the list with 44 and when we find the number ,no need to proceed further, So we can put a break statement in block of <strong>for loop</strong>. See below.</p>
<pre>
<code class="language-python">numbers_list=[5,2,44,10,25]
for i in numbers_list:
   if (i == 44):
       print(“Found”)
       Break</code></pre>
<p dir="ltr"><strong>Question</strong>: Write a program to find a sum of first five numbers from the given list numbers=[25, 33, 42, 28, 53, 66, 75, 36, 80, 40] and display an output as "Sum of first five number is &lt;answer&gt; ".</p>


### 💻 Solution (python):

```python
numbers = [25, 33, 42, 28, 53, 66, 75, 36, 80, 40]
count = 0
total = 0
for i in numbers:
  total = total + i
  count = count + 1
  if(count == 5):
    break
print("Sum of first five number is " + str(total))

```

---

## :question: Question 4 (Order: 4)

<p><u><strong>Nested loops</strong></u></p>
<p><meta charset="utf-8"/></p>
<p dir="ltr">If we define loops inside another loop is called nested loops.</p>
<p dir="ltr">For example, if we have a shapes as Pyramid and Sphere with colors as Blue, Green and Yellow and want to print shape details with its color variations, then code is as below and output is also as below.</p>
<pre>
<code class="language-python">shapes = ['Sphere', 'Pyramid']
colors = ['Blue', 'Green', 'Yellow']
for shape in shapes:
   print(shape)
   print("--------------------")
   for color in colors:        
       print(color + " " + shape)
   print("--------------------")
</code></pre>
<p><strong>Output:</strong></p>
<pre>
<code class="language-python">Sphere
--------------------
Blue Sphere
Green Sphere
Yellow Sphere
--------------------
Pyramid
--------------------
Blue Pyramid
Green Pyramid
Yellow Pyramid
--------------------</code></pre>
<p><strong>Question</strong>: Write a program that ask user for an input number, which is less than 25 and if entered number is present in num = [16, 8, 12, 5, 7, 10, 11, 9, 13, 15] then print numbers from 1 to the entered number otherwise print “Not found”.</p>


### 💻 Solution (python):

```python
num = [16, 8, 12, 5, 7, 10, 11, 9, 13, 15]
isPresent = False
input_num  = int(input())
for i in num:
  if i == input_num:
    isPresent = True
    for j in range(1, i + 1):
      print(j)
if(isPresent == False):
  print("Not found")
```

---

## :question: Question 5 (Order: 5)

<p><strong><u>The While Loop</u></strong></p>
<p><strong>While loop </strong>is an unlike a <strong>for loop</strong>, it repeats as long as a certain condition is True. When the python program execution reaches a <strong>while statement</strong>, it checks the condition next to the <strong>while keyword</strong>. If the condition evaluates to True, the execution moves inside the <strong>while block</strong>. If the condition evaluates to False, the execution moves past the <strong>while block</strong>.</p>
<p>For example, the program to increment the value of x and y based on the conditions like x&lt;35 and y&lt;50,</p>
<pre>
<code class="language-python">x = 28
y = 4

while (x &lt; 35 and y &lt; 50):
    x = x + 1
    y = y + 1
    print(x, y)</code></pre>
<p><strong>Output:</strong></p>
<pre>
<code class="language-python">29 45
30 46
31 47
32 48
33 49
34 50</code></pre>
<p><strong>Question:</strong> Write a program to print all the numbers between x and y (including x and y) where x and y is entered input.</p>


### 💻 Solution (python):

```python
x = int(input())
y = int(input())
num = 0
while(x <= y and num <= y):
  if(x <= num <= y):
    print(num)
  num = num + 1
```

---

