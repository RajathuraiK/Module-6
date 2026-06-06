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
