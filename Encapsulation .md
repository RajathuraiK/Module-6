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
