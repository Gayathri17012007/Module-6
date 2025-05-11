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
~~~c
from abc import ABC, abstractmethod
import math
class Shape(ABC):
    @abstractmethod
    def calculate_area(self):
        pass
class Rectangle(Shape):
    def __init__(self, width, height):
        self.width = width
        self.height = height
    
    def calculate_area(self):
        return self.width * self.height
class Circle(Shape):
    def __init__(self, radius):
        self.radius = radius
    def calculate_area(self):
        return math.pi * self.radius ** 2
rect = Rectangle(5, 4)
circle = Circle(3)
print("Area of Rectangle:", rect.calculate_area())
print("Area of Circle:", round(circle.calculate_area(), 2))
~~~

## Output
![Screenshot 2025-05-11 131826](https://github.com/user-attachments/assets/1d4c9f11-504b-4e07-b252-24d46a90901a)


## Result
Thus the program has been executed successfully.
