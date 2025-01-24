# 🚀 **Key Concepts in OOD**

### 📚 **Contents**

- **Coupling 🤝**
- **Cohesion 🔗**
- **The Four Pillars of OOAD 🏛️**
  - **Encapsulation 🔒**
  - **Abstraction 🌫️**
  - **Inheritance 🔁**
  - **Polymorphism ⚙️**


<br>

---


## **Coupling 🤝**
**Coupling** is about how much parts of a system depend on each other.

- **Tight coupling**: If one part needs a lot of help from others. Changes affect many things.
- **Loose coupling**: If parts can work mostly on their own. Changes affect less.

💡 In coding, we aim for **loose coupling** to make things easier to change 💡

<br>

---

## **Cohesion 🔗**
**Cohesion** is how well parts of a system work together to do one job.

- **High cohesion**: Everything in a part is focused on the same task.
- **Low cohesion**: Parts are tasks are scattered and not focused on the same task.

💡 We want **high cohesion** in code for clarity and easier maintenance 💡

<br>

---

## **The Four Pillars of OOD 🏛️**

Object-Oriented Analysis and Design (OOAD) revolves around four key ideas: **Encapsulation**, **Abstraction**, **Inheritance**, and **Polymorphism**. These ideas, also called **the Four Pillars of OOAD**, help make software systems more organized, flexible, and easy to maintain.

<br>

### → **🏛️ Encapsulation** 🔒: Keeping Things Safe 

**Encapsulation** is like having a box where the important things are hidden away. You don’t let anyone touch the important stuff directly, only through safe methods.

<br>

- **Example**: Imagine a `BankAccount` object. The balance is hidden inside the object, and you can only change it by calling `deposit()` or `withdraw()`.

```java
class BankAccount {
    private double balance;  // This is hidden away!

    public void deposit(double amount) {
        balance += amount;  // Safely add money
    }

    public double getBalance() {
        return balance;  // Get the balance, without messing with it
    }
}
```

#### **Why it's important 💡**
- Encapsulation is key to **data security** and **simplicity** in code.

<br>

.　 . • ☆ . ° .• °:. *₊ ° . ☆.　 . • ☆ . ° .• °:. *₊ ° . ☆.　 . • ☆ . ° .• °:. *₊ ° . ☆.　 . • ☆ . ° .• °:. *₊ ° . ☆.　 . • ☆ . ° .• °:. *₊ ° . ☆.　 . • ☆ . ° .• °:. *₊ ° . ☆

<br>

### → **🏛️ Abstraction** 🌫️: Hiding the Complicated Stuff 
**Abstraction** means you don’t need to know the complicated details. You just use what you need.

<br>

- **Example**: When you use a car, you don’t need to know how the engine works. You just press the gas pedal to go!

```java
abstract class Vehicle {
    public abstract void start();  // Just know it starts, no need to understand everything
}

class Car extends Vehicle {
    @Override
    public void start() {
        System.out.println("Car started!");
    }
}
```

#### **Why it's important 💡**
- Abstraction **simplifies** complex systems.
- By only exposing essential information and hiding unnecessary details, you make the code **easier** to understand and use.
  
<br>

.　 . • ☆ . ° .• °:. *₊ ° . ☆.　 . • ☆ . ° .• °:. *₊ ° . ☆.　 . • ☆ . ° .• °:. *₊ ° . ☆.　 . • ☆ . ° .• °:. *₊ ° . ☆.　 . • ☆ . ° .• °:. *₊ ° . ☆.　 . • ☆ . ° .• °:. *₊ ° . ☆

<br>

### → **🏛️ Inheritance** 🔁: Sharing Features 
**Inheritance** is like a family where children get traits from their parents. You don’t need to create everything from scratch!

<br>

- **Example**: A Vehicle class has basic features, and Car and Truck inherit those features, but they can also add their own.

```java
class Vehicle {
    public void move() {
        System.out.println("Moving...");
    }
}

class Car extends Vehicle {
    public void honk() {
        System.out.println("Beep beep!");
    }
}
```
#### **Why it's important 💡**
- Inheritance helps with code **reuse** and **reducing redundancy**

<br>

.　 . • ☆ . ° .• °:. *₊ ° . ☆.　 . • ☆ . ° .• °:. *₊ ° . ☆.　 . • ☆ . ° .• °:. *₊ ° . ☆.　 . • ☆ . ° .• °:. *₊ ° . ☆.　 . • ☆ . ° .• °:. *₊ ° . ☆.　 . • ☆ . ° .• °:. *₊ ° . ☆

<br>

### → **🏛️ Polymorphism** ⚙️: One Name, Many Actions 
**Polymorphism** means that one name can do different things! The same action can be done in different ways by different objects.

<br>

- **Example**: Both Car and Truck have a move() action, but they each do it in their own way.

```java
class Vehicle {
    public void move() {
        System.out.println("Moving...");
    }
}

class Car extends Vehicle {
    @Override
    public void move() {
        System.out.println("Car is zooming!");
    }
}

class Truck extends Vehicle {
    @Override
    public void move() {
        System.out.println("Truck is hauling!");
    }
}
```
#### **Why it's important 💡**
- Polymorphism enables **flexibility** and **extensibility** in your code.
- It allows you to use the same method name for different types of objects, letting you write more **generic** and **reusable** code.

<br>
