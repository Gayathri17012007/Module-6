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
~~~c
class Beans:
    def get_type(self):
        return "Vegetable"
    def get_color(self):
        return "Green"
class Mango:
    def get_type(self):
        return "Fruit"
    def get_color(self):
        return "Yellow"
def describe(item):
    print(f"Type: {item.get_type()}")
    print(f"Color: {item.get_color()}")
    print("-" * 20)
bean = Beans()
mango = Mango()
describe(bean)
describe(mango)
~~~

## Output
![Screenshot 2025-05-11 132827](https://github.com/user-attachments/assets/126625f8-7f0b-4fec-94f2-cca83e633c96)


## Result
Thus the program has been executed successfully.
