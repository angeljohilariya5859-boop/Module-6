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

from abc import ABC, abstractmethod
import math

# Abstract Class
class Shape(ABC):

    @abstractmethod
    def calculate_area(self):
        pass

# Rectangle Class
class Rectangle(Shape):
    def __init__(self, length, breadth):
        self.length = length
        self.breadth = breadth

    def calculate_area(self):
        return self.length * self.breadth

# Circle Class
class Circle(Shape):
    def __init__(self, radius):
        self.radius = radius

    def calculate_area(self):
        return math.pi * self.radius * self.radius


# Input for Rectangle
length = float(input("Enter Length of Rectangle: "))
breadth = float(input("Enter Breadth of Rectangle: "))

rect = Rectangle(length, breadth)
print("Area of Rectangle =", rect.calculate_area())

# Input for Circle
radius = float(input("Enter Radius of Circle: "))

cir = Circle(radius)
print("Area of Circle =", cir.calculate_area())
## Output
<img width="1918" height="912" alt="image" src="https://github.com/user-attachments/assets/3b6da926-f7fc-4e98-8e3d-1ef04e3908ab" />

## Result
Thus, The Python program to create an abstract class named Shape with an abstract method calculate_area, and implement this method in two subclasses: Rectangle and Circle was executed successfully.
