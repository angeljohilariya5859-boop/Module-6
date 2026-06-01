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
class A:
    def __init__(self,a):
        self.a = a
    def __lt__(self,other):
        if self.a < other.a:
            print(f"\n{self.a} is less than {other.a}")
        else:
            print(f"\n{self.a} is not less than {other.a}")

a = int(input())
b = int(input())
print("\nThe program to demonstrate operator overloading is executing........")
print("Operator overloading for overloading 'less than (<)' operator......")
ob1 = A(a)
ob2 = A(b)
ob1 < ob2
## Output
<img width="1919" height="908" alt="image" src="https://github.com/user-attachments/assets/357ccb2f-de74-4e17-86f3-77bfd78cfae2" />

## Result
Thus, The Python program that demonstrates operator overloading by overloading the less than (<) operator using a custom class was executed successfully.
