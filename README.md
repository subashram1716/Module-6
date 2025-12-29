## PYTHON PROGRAMING MODULE 6

# DATE: 20/12/2025

# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an *abstract class* named Shape with an *abstract method* calculate_area, and implement this method in two subclasses: Rectangle and Circle.

---

## 🧠 ALGORITHM
```
1. *Import ABC module*:
   - Use from abc import ABC, abstractmethod to define abstract classes and methods.

2. **Create Abstract Class Shape**:
   - Define an abstract method calculate_area() with @abstractmethod.

3. **Create Subclass Rectangle**:
   - Set default values for length and breadth.
   - Override calculate_area() to compute the rectangle area.

4. **Create Subclass Circle**:
   - Set default value for radius.
   - Override calculate_area() to compute the circle area.

5. *Create Objects & Call Methods*:
   - Instantiate Rectangle and Circle.
   - Call their calculate_area() methods.

---

## 💻 Program

from abc import ABC
class Shape(ABC):
    def calculate_area(self):
        pass
class Rectangle(Shape):
    length = 5
    breadth =3 
    def calculate_area(self):
        return self.length * self.breadth

class Circle(Shape):
  radius = 4
  def calculate_area(self):
      return 3.14 * self.radius * self.radius
rec=Rectangle()
rec.calculate_area()
cir=Circle()
cir.calculate_area()
print("Area of a rectangle:", rec.calculate_area()) #call to 'calculate_area' method defined inside the class 'Rectangle'
print("Area of a circle:", cir.calculate_area()) #call to 'calculate_area' method defined inside the class 'Circle'.
```
## Output
![WhatsApp Image 2025-10-19 at 20 18 56_6e030460](https://github.com/user-attachments/assets/9262ae2c-0a8e-41f4-92d5-f4048258e7ad)


## Result
The program successfully calculates area of shapes using abstarct method and classes
# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an *abstract class* named Shape with an *abstract method* calculate_area, and implement this method in two subclasses: Rectangle and Circle.

---

## 🧠 ALGORITHM
```
1. *Import ABC module*:
   - Use from abc import ABC, abstractmethod to define abstract classes and methods.

2. **Create Abstract Class Shape**:
   - Define an abstract method calculate_area() with @abstractmethod.

3. **Create Subclass Rectangle**:
   - Set default values for length and breadth.
   - Override calculate_area() to compute the rectangle area.

4. **Create Subclass Circle**:
   - Set default value for radius.
   - Override calculate_area() to compute the circle area.

5. *Create Objects & Call Methods*:
   - Instantiate Rectangle and Circle.
   - Call their calculate_area() methods.

---

## 💻 Program

from abc import ABC
class Shape(ABC):
    def calculate_area(self):
        pass
class Rectangle(Shape):
    length = 5
    breadth =3 
    def calculate_area(self):
        return self.length * self.breadth

class Circle(Shape):
  radius = 4
  def calculate_area(self):
      return 3.14 * self.radius * self.radius
rec=Rectangle()
rec.calculate_area()
cir=Circle()
cir.calculate_area()
print("Area of a rectangle:", rec.calculate_area()) #call to 'calculate_area' method defined inside the class 'Rectangle'
print("Area of a circle:", cir.calculate_area()) #call to 'calculate_area' method defined inside the class 'Circle'.
```
## Output
![WhatsApp Image 2025-10-19 at 20 18 56_6e030460](https://github.com/user-attachments/assets/9262ae2c-0a8e-41f4-92d5-f4048258e7ad)


## Result
The program successfully calculates area of shapes using abstarct method and classes
# 🐟 Method Overriding-Fish and Shark Class Inheritance in Python

## 🧠 AIM:
To write a Python program that demonstrates class inheritance by creating a parent class Fish with a method type, and a child class Shark that overrides the type method.

## 📋 ALGORITHM:

1. Define the Fish class with a method named type() that prints "fish".
2. Define the Shark class as a subclass of Fish, and override the type() method to print "shark".
3. Create an instance of the Fish class named obj_goldfish.
4. Create an instance of the Shark class named obj_hammerhead.
5. Use a for loop to iterate over both objects.
6. Within the loop, call the type() method using the loop variable.
7. Output will demonstrate method overriding: printing "fish" and "shark" accordingly.

## 💻 PROGRAM:
```
class Fish:
       def type(self):
           print("fish")
class Shark(Fish):
	   def type(self):
	       print("shark")

obj_goldfish=Fish()
obj_hammerhead=Shark()
#Call the functions for fish and shark class using the objects
obj_goldfish.type()
obj_hammerhead.type()
```
## OUTPUT
![WhatsApp Image 2025-10-19 at 20 29 36_6bc6f810](https://github.com/user-attachments/assets/642edbb8-6d46-4d60-9eb6-357f2f79a786)


## RESULT
The program successfully creates class inheritance
# 🐍 Python OOP: Operator Overloading (Less Than `<`)

## 🎯 AIM

To write a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.

---

## 🧠 ALGORITHM

1. **Create Class `A`**:
   - Define the `__init__()` method to initialize the object with a value `a`.

2. **Overload the `<` Operator**:
   - Define the `__lt__()` method with logic:
     - If `self.a < o.a`, return `"ob1 is less than ob2"`
     - Else, return `"ob2 is less than ob1"`

3. **Create Objects**:
   - Instantiate two objects `ob1` and `ob2` with values.

4. **Use `<` Operator**:
   - Use `print(ob1 < ob2)` to trigger the overloaded behavior.

---

## 💻 Program
```
class A:
    def _init_(self, value):
        self.value = value
    def _lt_(self, other):
        return self.value < other.value

ob1 = A(200)
ob2 = A(30)
if ob1 < ob2:
    print("ob1 is less than ob2")
else:
    print("ob2 is less than ob1")
```


## Output
![WhatsApp Image 2025-10-19 at 20 26 10_8fd2d08a](https://github.com/user-attachments/assets/4b36bf4b-a461-4627-a987-aba3e3be4e64)


## Result
The program successfully demonstrates operator overloading by redefining the less than (<) operator in a custom class.
When comparing two objects, the overloaded method __lt__() executes, producing a descriptive comparison result instead of a boolean value.
# # 🐍 Python OOP: Polymorphism with Classes

## 🎯 AIM

To create two specific classes — Beans and Mango. Then, create a *generic function* that can accept any object and determine its *type* (Fruit or Vegetable) and *color*, using polymorphism.

---

## 🧠 ALGORITHM

1. **Create Class Beans**:
   - Define type() method that prints "Vegetable".
   - Define color() method that prints "Green".

2. **Create Class Mango**:
   - Define type() method that prints "Fruit".
   - Define color() method that prints "Yellow".

3. **Define Generic Function func(obj)**:
   - Call obj.type() and obj.color() — this works with both Beans and Mango objects, showcasing *polymorphism*.

4. *Create Objects*:
   - Instantiate Beans and Mango.
   - Pass them to func() and execute the program.

---

## 💻 Program
```
class Beans(): 
    def f(self):
        print("Vegetable")
        print("Green")
class Mango(): 
    def d(self):
        print("Fruit")
        print("Yellow")
     #Add your code here      
def func(obj): 
    pass
       #Add your code here
#creating objects
o = Beans() 
o.f()
ob = Mango() 
ob.d()

```
## Output
![WhatsApp Image 2025-10-19 at 20 55 13_5c1b6e79](https://github.com/user-attachments/assets/997c9553-dcea-48fc-be5a-27df9dacb4ad)


## Result
The program successfully creates class and returns type  using polymorphism
