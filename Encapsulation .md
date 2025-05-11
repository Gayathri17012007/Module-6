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
~~~c
class Rectangle:
    def __init__(self, length, breadth):
        self.__length = length    
        self.__breadth = breadth   
    def get_length(self):
        return self.__length
    def set_length(self, length):
        if length > 0:
            self.__length = length
        else:
            print("Length must be positive.")
    def get_breadth(self):
        return self.__breadth
    def set_breadth(self, breadth):
        if breadth > 0:
            self.__breadth = breadth
        else:
            print("Breadth must be positive.")
    def calculate_area(self):
        return self.__length * self.__breadth
rect = Rectangle(10, 5)
print("Length:", rect.get_length())
print("Breadth:", rect.get_breadth())
print("Area:", rect.calculate_area())
rect.set_length(-3)
rect.set_breadth(7)
print("\nUpdated Length:", rect.get_length())
print("Updated Breadth:", rect.get_breadth())
print("Updated Area:", rect.calculate_area())
~~~
## Output
![Screenshot 2025-05-11 132144](https://github.com/user-attachments/assets/8ef271ce-a94f-49e1-9f45-7fde90158418)


## Result
Thus the program has been executed successfully.
