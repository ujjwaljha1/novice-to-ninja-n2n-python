# 📚 Questions for ID: 5bad1b2aa2da6b25b98780d1

## :question: Question 1 (Order: 1)

<p>Write a program to define a class as Temprature which contains two methods as celseiusToFahren() and fahrenToCelseius()  as below and display the output by creating its object and calling its methods. The first method takes 10 degree celsius and the second method takes 100 degree fahrenheit as an input.</p>
<p>1) The celseiusToFahren() method, which takes celsius value, converts it into fahrenheit and print resulted fahrenheit value upto 1 decimal point (eg. 50.0).</p>
<p>2) The fahrenToCelseius() method,which takes fahrenheit value, converts it into celsius and print resulted celsius value upto 1 decimal point (eg. 50.0).</p>
<p><strong>Hint: </strong>Formula of<strong> </strong> Fahrenheit = (celsius *  9.0 / 5.0 ) + 32</p>


### 💻 Solution (python):

```python
class Temperature():
  def celseiusToFahren(self, celsius):
    self.celsius = float(celsius)
    self.fahren = (celsius *  9.0 / 5.0 ) + 32
    print("%.1f"%(self.fahren))
  def fahrenToCelseius(self, fahren):
    self.fahren = fahren
    self.celsius = (fahren - 32) * 5.0 / 9.0
    print("%.1f"%(self.celsius))
    
temp = Temperature()
temp.celseiusToFahren(10)
temp.fahrenToCelseius(100)
```

---

## :question: Question 2 (Order: 2)

<p>Write a program to define a class Student which is initialized with two variables as (name and roll_number) and contains two methods as display_info() and setMarks() as below.</p>
<p><meta charset="utf-8"/></p>
<p dir="ltr">1)The display_info() method, which display the Name and Roll No of student in separate lines.</p>
<p dir="ltr">2)The setMarks() method , which assign a marks to the student and display the Marks of  the student.</p>
<p dir="ltr">The output should be displayed the student details as Name, Roll No and Marks in separate lines by creating an object and calling methods of a Student class.</p>
<p dir="ltr">Take input as Name=Emma, Roll no=18 and Marks=68.</p>


### 💻 Solution (python):

```python
class Student():
  def __init__(self, name, roll_no):
    self.name = name
    self.roll_no = roll_no
  def display_info(self):
    print("Name: " + self.name)
    print("Roll no: " + str(self.roll_no))
  def setMarks(self, marks):
    self.marks = marks
    print("Marks: " + str(self.marks))   
    
student1 = Student("Emma", 18)
student1.display_info()
student1.setMarks(68)
```

---

## :question: Question 3 (Order: 3)

<p><meta charset="utf-8"/>Write a program to define a class Date, which is initialized with 3 variables as (date, month and year) and containts a method as print_date, which display the date in format as "day month year" (eg: 12 January 2020). The output should be displayed the date value by creating an object of a Date class and calling its method. Consider input date= 8/April/2000.</p>


### 💻 Solution (python):

```python
class Date:
    def __init__(self, d, m, y):
        self.date = d
        self.month = m
        self.year = y
        
    def print_date(self):
        print(self.date + " " + self.month + " " + self.year)
        
Date1 = Date("08", "April", "2000")
Date1.print_date()
```

---

## :question: Question 4 (Order: 4)

<p>Write a program to define a class Fruits, which is initialized with name and price of fruit ,and contains a two methods as below.</p>
<p>1) A method, which assign a quantity for fruit and print the value of it. Consider the fixed quantity as 10 for fruit.<br/>
2) A method , which calculate the total price of fruit and print the value of it.</p>
<p>The output should be print the quantity and total price of Apple in separate lines, if a price per apple is 50. To get an output, create an object of a Fruits class and call methods of it.</p>


### 💻 Solution (python):

```python
class Fruits:
    def __init__(self, n, p):
        self.name = n
        self.price = p
        
    def quantity(self):
        self.quantity = 10
        print(self.quantity)
    
    def total_price(self):
        self.total_price = self.quantity * int(self.price)
        print(self.total_price)
        
Fruit1 = Fruits("Apple", "50")
Fruit1.quantity()
Fruit1.total_price()
```

---

## :question: Question 5 (Order: 5)

<p>Write a program to perform the followings for the given class Animals and its methods as eat and walk, which prints "Eating...." and "Walking....". respectively. </p>
<p>1) Create a two classes Herbivores and Carnivores as a subclass of the class Animals, which has eating method as herb_eat() and carn_eat() respectively.</p>
<p>2) The herb_eat() method use the eat() method of Animals class and prints Grass.</p>
<p>3) The carn_eat() method use the eat() method of Animals and prints Meat.</p>
<p>4) Create an object as cow for a Herbivores class and call the herb_eat() method to get the output.</p>
<p>5) Create an object as lion for a Carnivores class and call the carn_eat() method to get the output.</p>


### 💻 Solution (python):

```python
class Animals:            
    def eat(self):
        print("Eating....")
    
    def walk(self):
        print("Walking.....")

class Herbivores(Animals): 
    def herb_eat(self):
        self.eat()
        print("Grass")

class Carnivores(Animals):
    def carn_eat(self):
        self.eat()
        print("Meat")

cow = Herbivores()
cow.herb_eat()
lion = Carnivores()
lion.carn_eat()
```

---

## :question: Question 6 (Order: 6)

<p>Write a program to define a class Rectangle, which is initialized by a length and a width and contains a method, which calculates the area of rectangle and print the result of it. The output should be displayed the area of rectangle for length=5 and width=12 by creating a object of a Rectangle class and calling a method of it.<br/>
 </p>


### 💻 Solution (python):

```python
class Rectangle():
    def __init__(self, l, w):
        self.length = l
        self.width  = w

    def findArea(self):
        return self.length * self.width

rect1 = Rectangle(5,12)
print(rect1.findArea())
```

---

## :question: Question 7 (Order: 7)

<p>Write a program to define a class Shape and its subclass Square. The Square class has a function as init, which takes a length as an argument. Both classes have a function as an 'area', which calculates and returns an area of the shape. By default , take area of Shape class is 0. The output should be displayed the area of square for length=5 by creating an object of a Square class and calling its method.<br/>
 </p>


### 💻 Solution (python):

```python
class Shape():
    def __init__(self):
        pass

    def area(self):
        return 0

class Square(Shape):
    def __init__(self, l):
        self.length = l

    def area(self):
        return self.length * self.length

sq1= Square(5)
print(sq1.area())


```

---

## :question: Question 8 (Order: 8)

<p>Write a program to define a class Person with its two child classes as Male and Female. All 3 classes have a method getGender(), which will print the "Male" for Male class, "Female" for Female class and "Unknown" for Person class.The output should be displayed a "Male" and "Female" in separate lines against creating an object of a childclass of a Person class and calling getGender()method.<br/>
 </p>


### 💻 Solution (python):

```python
class Person():
    def getGender(self):
        return "Unknown"

class Male(Person):
    def getGender(self):
        return "Male"

class Female(Person):
    def getGender(self):
        return "Female"

male_obj = Male()
female_obj = Female()
print(male_obj.getGender())
print(female_obj.getGender())

```

---

## :question: Question 9 (Order: 9)

<p>Write a program to define a class called Poem which is initialized with variable poem, which includes below poem lines as a list and contains a method as getPoem(),which prints the each line of poem.</p>
<p>When I behold a forest spread<br/>
With silken trees upon thy head;<br/>
And when I see that other dress<br/>
Of flowers set in comeliness;</p>
<p>The output should be displayed the all lines of a poem in separate lines by creating an object of a Poem class and calling its method.</p>


### 💻 Solution (python):

```python
class Poem():
    def __init__(self):
        self.poem = ["When I behold a forest spread", "With silken trees upon thy head;", "And when I see that other dress", "Of flowers set in comeliness;"]

    def getPoem(self):
      for line in self.poem:
        print(line)
obj = Poem()
obj.getPoem()
```

---

