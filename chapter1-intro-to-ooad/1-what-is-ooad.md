# 🚀 **What is OOAD?**

## **What is OOAD?**
**Object-Oriented Analysis and Design (OOAD)** is a way to plan and build software using **objects**. Think of it like organizing your code into small, easy-to-manage pieces that each do something useful.

<br>

---

## **Vocabulary in OOAD**

### **1. 🧸 Objects and 🏗️ Classes**
- **Objects**: These are like real-world things. For example, a `cat` is an object.
- **Classes**: These are like blueprints or plans for creating objects. A `Cat` class would be the blueprint to create different cats (objects).

For example:
```java
class Cat {
    String name;  
    String color; 
    int age;       

    public void meow() {
        System.out.println("Meow!");
    }
}
```

Here, `Cat` is the class (blueprint), and each `Cat` object can have different names, colors, and ages, but they all can meow!

<br>

### 2. 🏷️ Attributes and 🔧 Methods
- **Attributes**: These are the **properties** of the object. For example, `name`, `color`, and `age` are **attributes** of the Cat object.
- **Methods**: These are the **actions** the object can do. For example, `meow()` is a **method** that tells the cat to meow.

In the previous code example:  
For example:

```java
class Cat {
    String name;  // This is an attribute (characteristic) of the cat
    String color; // Another attribute
    int age;       // Another attribute
    
    // This is a method (action) the cat can do
    public void meow() {
        System.out.println("Meow!");
    }
}
```

<br>

---

## Why Use OOAD?

- **🔩 Modular**: It makes big projects easier to work on because you break them into small parts (objects).
- **♻️ Reusable**: You can use the same objects in many parts of your code.
- **⚙️ Easier to Manage**: It's simpler to change or fix things because each object works on its own.
  
With OOAD, you create organized, manageable, and reusable code that’s easier to update or fix later on.
