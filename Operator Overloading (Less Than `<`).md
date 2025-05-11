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
~~~c
class Box:
    def __init__(self, volume):
        self.volume = volume
    def __lt__(self, other):
        return self.volume < other.volume
box1 = Box(100)
box2 = Box(150)
if box1 < box2:
    print("Box 1 is smaller than Box 2.")
else:
    print("Box 1 is not smaller than Box 2.")
~~~

## Output
![Screenshot 2025-05-11 132615](https://github.com/user-attachments/assets/e1f849ec-2b98-4371-986e-68c19d839101)


## Result
Thus,the program has been executed successfully.
