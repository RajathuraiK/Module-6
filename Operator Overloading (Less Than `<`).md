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

