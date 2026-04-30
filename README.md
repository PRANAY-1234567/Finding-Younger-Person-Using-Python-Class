# 👤 Finding Younger Person Using Python Class (OOP)

## 📌 Description

This Python program demonstrates how to **compare two objects** and return one based on a condition. It finds the **younger person** between two `Person` objects.

---

## 🚀 Features

* Defines a `Person` class
* Stores name and age
* Compares two objects
* Returns the younger person
* Displays result

---

## 🛠️ How It Works

1. A class `Person` is created with:

   * `name`
   * `age`

2. Methods:

   * `getInfo()` → Displays person details
   * `younger(t)` →

     * Compares current object (`self`) with another object `t`
     * Returns the object with smaller age

3. In the main program:

   * Two objects `p1` and `p2` are created
   * `younger()` method is called
   * Result is stored in `y`
   * Details of younger person are displayed

---

## 💻 Code

```python id="h3x9pt"
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def getInfo(self):
        print("Name  :", self.name)
        print("Age   :", self.age)

    def younger(self, t):
        if self.age < t.age:
            return self
        else:
            return t
        
p1 = Person("Akshay", 26)
p2 = Person("Saurabh", 30)

y = p1.younger(p2)

print("Younger Person")
y.getInfo()
```

---

## ▶️ Example Output

```id="q2l7mv"
Younger Person
Name  : Akshay
Age   : 26
```

---

## 📚 Concepts Used

* Class and Object
* Passing object as argument
* Returning object from method
* Conditional statements

---

## 🧠 Key Concept

👉 `self` → current object (`p1`)
👉 `t` → object passed as argument (`p2`)

The method returns **one of the objects**, not just a value.

---

## 🎯 Use Case

This helps you understand:

* How objects can be compared
* How methods can return objects
* Real-world logic implementation

---

## 🔧 Future Improvements

* Compare more than two persons
* Find oldest person
* Add list of persons and find youngest using loop
* Use `min()` with custom key

---

## 📄 License

This project is open-source and free to use.

<img width="1273" height="701" alt="image" src="https://github.com/user-attachments/assets/2d560712-7a61-4dd9-811b-2bb9bbe4aedb" />

