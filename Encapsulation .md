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
class Rectangle:
    # Constructor
    def __init__(self, length, breadth):
        self.__length = length      # Private member
        self.__breadth = breadth    # Private member

    # Method to display details
    def display(self):
        print("Length :", self.__length)
        print("Breadth :", self.__breadth)

    # Method to calculate area
    def area(self):
        return self.__length * self.__breadth


# Input
length = float(input("Enter Length: "))
breadth = float(input("Enter Breadth: "))

# Object Creation
r = Rectangle(length, breadth)

# Display Details
r.display()
print("Area =", r.area())
   
## Output
<img width="1917" height="912" alt="image" src="https://github.com/user-attachments/assets/6aa01bc5-5699-41bd-a6b9-77f312f3652e" />

## Result
Thus, The Python program to implement Encapsulation in Python by defining a class Rectangle with private member variables __length and __breadth. was executed successfully.
