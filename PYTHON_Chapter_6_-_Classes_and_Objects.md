# 📚 Questions for ID: 5baa729e4813f0a1c5497a17

## :question: Question 1 (Order: 1)

<p>In a procedural programming, the entire code is written into one long procedure even though it might contain functions and subroutines. It is not manageable as both data and logic, get mixed together. But when we talk about object-oriented programming, the program is split into self-contained objects or several mini-programs.</p>
<p><meta charset="utf-8"/></p>
<p dir="ltr">When working on complex programs in particular, objects are a way of organizing code in a program and breaking things down to make it easier to think about complex ideas.The object-oriented programming makes your code more readable, which in turn makes it more maintainable.</p>
<p>Python is an object-oriented programming language. One of the most important concepts in object-oriented programming is the distinction between classes and objects, which are defined as follows:</p>
<p>Class --&gt; A blueprint created by a programmer for an object. This defines a set of properties that will characterize any object. We can think of class as a way to classify objects into groups.</p>
<p dir="ltr">Object --&gt; An instance of a class. This is the realized version of the class, where the class is manifested in the program.</p>
<p>For example: let’s think of humans as a class which posses a set of properties like name ,age etc. then we all are different instances, that are objects of the class human, with different properties like name and age.</p>
<p><strong>Question:</strong> _____ represents an entity in the real world with its identity and behaviour.</p>
<p dir="ltr">a) A method</p>
<p dir="ltr">b) An object</p>
<p dir="ltr">c) A class</p>
<p dir="ltr">d) An operator</p>


### 📝 Answer Options:

1. ❌ 
<p>A method</p>


2. ✅ **Correct Answer:**
<p dir="ltr">An object</p>


3. ❌ 
<p>A class</p>


4. ❌ 
<p>An operator</p>


---

## :question: Question 2 (Order: 2)

<p><strong><u>Defining classes, objects and class methods</u></strong></p>
<p>A class in python is the blueprint from which specific objects are created.</p>
<p>We start the class definition with the class keyword, followed by the class name and a colon.</p>
<pre>
<code class="language-python">class Lion:
      pass</code></pre>
<p>In above code, class name is Lion and pass is a block of code of class Lion. The pass statement in python is used when a statement is required syntactically but we don't want any command or code to execute. The pass statement is a null operation; nothing happens when it executes.</p>
<p>With the same blueprint (ie, class), we can create several instances and these can be considered as Objects  Like we can take the Lion class defined above and use it to create an object or instance of it.</p>
<p>jake = Lion()</p>
<p>Here, we initialized the object 'Jake' as an instance of the class by setting it equal to Lion()</p>
<p>Now creating a class is incomplete without some functionality. So functionalities can be defined by setting various attributes which acts as a container for data and functions related to those attributes.</p>
<pre>
<code class="language-python">class Lion:

   def walk(self):
        print("The lion is walking")

   def roar(self):
        print("The lion is roaring")

jake = Lion()</code></pre>
<p>In the above code, we defined a two functions walk() and roar() for the class Lion because these functions are indented under the class Lion, they are called methods. Methods are a special kind of function that are defined within a class.</p>
<p>In next lesson, we will discuss more about the parameter self used in function (method) definition.</p>
<p><strong>Question:</strong> Write a code to perform the followings. </p>
<p>1) Define a class named Bird </p>
<p>2) Add a function named fly which print message as "The bird is flying".</p>
<p>3) Create an object of class Bird and call the function to get the output as The bird is flying.</p>


### 💻 Solution (python):

```python
class Bird:
	def fly(self):
		print("The bird is flying")

b1 = Bird() #making object
b1.fly() #calling function fly
```

### 📝 Answer Options:

1. ❌ 


2. ❌ 


3. ❌ 


4. ❌ 


---

## :question: Question 3 (Order: 3)

<p><u><strong>Methods Attributes and Self Keyword</strong></u></p>
<pre>
<code class="language-python">class Lion:
    def walk(self):
        print("The lion is walking")

    def roar(self):
        print("The lion is roaring")
jake = Lion()</code></pre>
<p><span style="font-family:Arial,Helvetica,sans-serif;">In the above example, we initialized the object jake as an instance of the class Lion. There is a new keyword self in the function definition, which was not present in the normal function definition. As soon as we define a new class  and a new class object is created with the same name. This class object allows us to access the different attributes of that class. To access its own properties we use the keyword self, It is mandatory to pass self as a parameter ,if the method is inside the class.</span></p>
<p><span style="font-family:Arial,Helvetica,sans-serif;">let’s use the two methods  of class Lion with the object jake as below.</span></p>
<pre>
<code class="language-python">jake = Lion()
jake.walk()
jake.roar()</code></pre>
<p>And output would be like,<br/>
The lion is walking<br/>
The lion is roaring</p>
<p><span style="font-family:Arial,Helvetica,sans-serif;">The class Lion using the two methods walk() and roar(). We called these using the dot operator (.), which is used to reference an attribute of an object. In this case, the attribute is a method and it’s called with parentheses like jake.walk()</span></p>
<p><span style="font-family:Arial,Helvetica,sans-serif;">Because the keyword self was a parameter of the methods as defined in the Lion class, the jake object gets passed to the methods. The self parameter ensures that the methods have a way of referring to object attributes. When we call the methods, however, nothing is passed inside the parentheses, the object jake is being automatically passed with the dot operator.</span></p>
<p><span style="font-family:Arial,Helvetica,sans-serif;"><strong>Question</strong>: Write a program to define a class Computer, with two methods system_in() and system_out() as below.</span></p>
<p><span style="font-family:Arial,Helvetica,sans-serif;">1) The method system_in() should ask for a username as an input and print string as "Welcome username".</span></p>
<p><span style="font-family:Arial,Helvetica,sans-serif;">2) The system_out() should display the string  as “Thank you for coming”. </span></p>
<p><span style="font-family:Arial,Helvetica,sans-serif;">The output should be display by creating an instance of the class and call the methods.</span></p>
<p><font face="Arial, Helvetica, sans-serif"><strong>Note:</strong> If username=John so output should be Welcome John and Thank you for coming!! in separate lines</font></p>


### 💻 Solution (python):

```python
class Computer:
    def system_in(self):
        Name=input()
        print("Welcome"+" "+ Name)
    def system_out(self):
        print("Thank you for coming!!")
        
sys1 = Computer()
sys1.system_in()
sys1.system_out()

```

---

## :question: Question 4 (Order: 4)

<p><u><strong>__init__() : The Constructor Method</strong></u></p>
<p>The constructor method is used to initialize data. It is run as soon as an object of a class is  created. Also known as the __init__ method, it will be the first definition of a class and looks like this:</p>
<pre>
<code class="language-python">class Lion:
      def __init__(self):
             print("This is the constructor method.")</code></pre>
<p>If we add the above __init__ method to the Lion class in the previous example, the program would execute the print statement inside the constructor method, whenever we create a new object.</p>
<p>Let’s create a constructor method for Student class that passes parameters to assign a variables to an object.</p>
<pre>
<code class="language-python">class Student:
    def __init__(self, first, last, roll_no):
        self.first_name = first
        self.last_name = last
        self.roll_no = roll_no
    
    def exam(self):
        reister_no = self.first_name + str(self.roll_no)
        print("Exam registration number is: " + "2018" + reister_no)

student1 = Student('Sophia', 'John', 5)
print(student1.first_name)
student1.exam()

Output:
Aleena
Exam registration number is: 2018Aleena5</code></pre>
<p>In the above code, a first, last and roll_no is used as a parameters of a constructor and we can set first name, last name and roll number to them using self keyword. Self is the instance which means whenever we write self.first_name = first, it is the same as student1.first_name = “Amal” ,where we have used instances of Student class as student1 and pass the values specified in the __init__() method. The __init__() method takes the instances as an arguments always. Instead of doing it manually, it will be done automatically now. The exam() method is defined to generate a registration number for each student. After executing the above code, the output shows as name of a person with registration number.</p>
<p><strong>Question:</strong> Write a program to create a constructor for a Circle class, which initialize with radius and includes two methods as find_area() and find_circumference() to find the area of a circle and find the circumference of a circle respectively.The output shows the result of area and circumference by creating an object of a class Circle and calling methods of it.</p>


### 💻 Solution (python):

```python
class Circle:
    def __init__(self, r):
        self.radius = r
        
    def find_area(self):
        self.area = 3.14 * self.radius * self.radius
        print("Area: %.1f"%(self.area))
    
    def find_circumference(self):
        self.circumference = 2 * 3.14 * self.radius
        print("Circumference: %.1f"%(self.circumference))
        
cir = Circle(10)
cir.find_area()
cir.find_circumference()
```

---

## :question: Question 5 (Order: 5)

<p><strong><u>Inheritance</u></strong><br/>
If a class is a part of another class, then it’s a child of that class and the other class is its parent. Classes can be both children of and parents to other classes.</p>
<pre>
<code class="language-python">class Children():
    pass
class Student(Children):
    pass</code></pre>
<p>Inheritance is when a class uses code,which constructed within another class. If we think of inheritance in terms of biology, we can think of a child inheriting certain traits from their parent. That is, a child can inherit a parent’s height or blood group. Children also may share the same last name with their parents. </p>
<p>Classes called child classes or subclasses are inherited methods and variables from parent classes or base classes. We can think of a parent class called Parent, that has a variables for last_name, height and blood group ,which child class called Child can inherit from the Parent. Because the Child subclass is inheriting from the Parent base class, the Child class can reuse the code of Parent, allowing the programmer to use fewer lines of code and decrease the redundancy.</p>
<p>For example,  we define a class Polygon as a parent class and initiate it with the list containing sides of the shape, which is 0. Define a method, inputSides(), to change the values of the list for this class.</p>
<pre>
<code class="language-python">class Polygon:
    def __init__(self, no_of_sides):
        self.n = no_of_sides
        self.sides = [0 for i in range(no_of_sides)]
        
    def inputSides(self):
        self.sides = [float(input("Enter side "+str(i+1)+" : ")) for i in range(self.n)]</code></pre>
<p>Now, we define another class Square with number of sides 4. Square is a child class of the class Polygon. Inside class definition, define a method to find area of the shape.</p>
<pre>
<code class="language-python">class Square(Polygon):
    def __init__(self):
        Polygon.__init__(self,4)
        
    def findArea(self):
        a = self.sides[0]
        self.area = a * a
        print("Area is " + str(self.area))</code></pre>
<p>Next, create an object 's' for Square class to find an area of the square. To get the output, we should give the input values for the sides, which can be done by calling inputSides() method of the parent class and then find the area of the square by calling findArea() method of the child class.</p>
<pre>
<code class="language-python">s = Square()
s.inputSides()
s.findArea()</code></pre>
<p><strong>Question</strong>: Following details are given.</p>
<p>1) Created a super class Person which is initiated with name and includes a method to check, if this person is a student or not.</p>
<p>2) Created an object of a child class and called method to get the output. The output shows person details, if the person is a student otherwise print "Data not available".</p>
<p>Write a program to define a child class Student with its methods by performing below instructions.</p>
<p>1) Create a new class Student which is a child class of Person and initiated with roll_no and gender. It inherrit the constructor of parent class ,where name=Sam.</p>
<p>2)This class includes a two methods as below.</p>
<p>       i) An isStudent() method is used to check a person is a student or not and return a True value for that.</p>
<p>       ii) A displayInfo() method  is used to print the personal information of student like name, roll number and gender as expected output.</p>
<p> </p>


### 💻 Solution (python):

```python
class Person:
    def __init__(self, name):
        self.name = name
        
    def isStudent(self):
        self.isStudent = False

class Student(Person):
    def __init__(self, roll_no, gender):
        Person.__init__(self, 'Sam')
        self.roll_no = roll_no
        self.gender = gender
        
    def isStudent(self):
        self.isStudent = True
        return self.isStudent
    
    def displayInfo(self):
        print("Name: " + self.name)
        print("Roll number: " + str(self.roll_no))
        print("Gender: " + self.gender)
        
student1 = Student(15, "Male")
if(student1.isStudent()):
  student1.displayInfo()
else:
  print("Data not available")
```

---

