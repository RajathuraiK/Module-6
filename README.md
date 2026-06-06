# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program

```
from abc import ABC, abstractmethod
import math

class shape(ABC):
    @abstractmethod
    def calculate_area(self):
        pass
class Rectangle(shape):
    def __init__(self,l=1,b=2):
        self.l=l
        self.b=b
    def calculate_area(self):
        return self.l*self.b
class Circle(shape):
    def __init__(self,r=3):
        self.r=r
    def calculate_area(self):
        return self.r*self.r*math.pi

rect=Rectangle(5,6)
cir=Circle(10)
print(rect.calculate_area())
print(f"{cir.calculate_area():.2f}")
```

## Output

<img width="908" height="327" alt="image" src="https://github.com/user-attachments/assets/65b10845-d181-4b32-ae85-860362b6cbd1" />


## Result

The python program to create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle` is successfully developed and executed.

# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program

```
class Rectangle:
    def __init__(self,l,b):
        self.__length=l
        self.__breadth=b
        print(f"The length of the rectangle is {self.__length} units and the breadth of the rectangle is {self.__breadth} units")

rect=Rectangle(15,8)
```

## Output

<img width="907" height="310" alt="image" src="https://github.com/user-attachments/assets/305a2e35-956e-4ade-acf6-e218e43b68d0" />


## Result

The python program to implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth` is successfully developed and executed.

# 🐟 Method Overriding-Fish and Shark Class Inheritance in Python

## 🧠 AIM:
To write a Python program that demonstrates class inheritance by creating a parent class `Fish` with a method `type`, and a child class `Shark` that overrides the `type` method.

## 📋 ALGORITHM:

1. Define the `Fish` class with a method named `type()` that prints `"fish"`.
2. Define the `Shark` class as a subclass of `Fish`, and override the `type()` method to print `"shark"`.
3. Create an instance of the `Fish` class named `obj_goldfish`.
4. Create an instance of the `Shark` class named `obj_hammerhead`.
5. Use a `for` loop to iterate over both objects.
6. Within the loop, call the `type()` method using the loop variable.
7. Output will demonstrate method overriding: printing `"fish"` and `"shark"` accordingly.

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
for obj in (obj_goldfish,obj_hammerhead):
    obj.type()
```

## OUTPUT

<img width="912" height="284" alt="image" src="https://github.com/user-attachments/assets/ed731c3e-30d3-45dc-8459-0b58d2038ae9" />


## RESULT

The python program to write a Python program that demonstrates class inheritance by creating a parent class `Fish` with a method `type`, and a child class `Shark` that overrides the `type` method is successfully developed and executed.

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
    def __init__(self,a):
        self.a=a
    def __lt__(self,other):
        if self.a<other.a:
            print("ob1 is less than ob2")
        else:
            print("ob2 is less than ob1")

a=A(17)
b=A(14)
a<b
```

## Output

<img width="912" height="283" alt="image" src="https://github.com/user-attachments/assets/8481bb84-a132-4067-bafd-878b386327ce" />


## Result

The python program to write a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class is successfully developed and executed.

# # 🐍 Python OOP: Polymorphism with Classes

## 🎯 AIM

To create two specific classes — `Beans` and `Mango`. Then, create a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism.

---

## 🧠 ALGORITHM

1. **Create Class `Beans`**:
   - Define `type()` method that prints `"Vegetable"`.
   - Define `color()` method that prints `"Green"`.

2. **Create Class `Mango`**:
   - Define `type()` method that prints `"Fruit"`.
   - Define `color()` method that prints `"Yellow"`.

3. **Define Generic Function `func(obj)`**:
   - Call `obj.type()` and `obj.color()` — this works with both `Beans` and `Mango` objects, showcasing **polymorphism**.

4. **Create Objects**:
   - Instantiate `Beans` and `Mango`.
   - Pass them to `func()` and execute the program.

---

## 💻 Program

```
class Beans:
    def type(self):
        print("Vegetable")
    def color(self):
        print("Green")
class Mango:
    def type(self):
        print("Fruit")
    def color(self):
        print("Yellow")
def func(obj):
    obj.type()
    obj.color()
beans=Beans()
mango=Mango()
for obj in (beans,mango):
    func(obj)
```

## Output

<img width="910" height="348" alt="image" src="https://github.com/user-attachments/assets/1fb65bc8-8425-40af-a726-a218e0e9d3c3" />


## Result

The python program to create two specific classes — `Beans` and `Mango`. Then, create a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism is successfully developed and executed.
