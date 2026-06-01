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
class Beans:
    def type(self):
        print("Vegetable")
    def colour(self):
        print("Green")
class Mango:
    def type(self):
        print("Fruit")
    def colour(self):
        print("Yellow")
def func(obj):
    obj.type()
    obj.colour()
    print()
ob1 = Beans()
ob2 = Mango()
func(ob1)
func(ob2)
## Output
<img width="1918" height="902" alt="image" src="https://github.com/user-attachments/assets/973c440a-2e43-431e-8f82-31e5fd87fba7" />

## Result
Thus, The Python program to create two specific classes — Beans and Mango. Then, create a generic function that can accept any object and determine its type (Fruit or Vegetable) and color, using polymorphismwas executed successfully.
