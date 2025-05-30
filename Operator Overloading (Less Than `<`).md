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
    def __init__(self, value):
        self.value = value

    def __lt__(self, other):
        if self.value < other.value:
            print(f"{self.value} is less than {other.value}")
            return True
        else:
            print(f"{self.value} is not less than {other.value}")
            return False

ob1 = A(20)
ob2 = A(3)

if ob2 < ob1:
    print("ob2 is less than ob1")
else:
    print("ob2 is not less than ob1")
```

## Output
![image](https://github.com/user-attachments/assets/827b5883-f18d-402a-9708-d23cad8c9185)


## Result
Thus the code is executed successfully.
