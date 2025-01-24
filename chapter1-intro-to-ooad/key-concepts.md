# 🚀 **Key Concepts in OOAD**

There are four key ideas in OOD: **Encapsulation**, **Abstraction**, **Inheritance**, and **Polymorphism**. These are often referred to as **the Four Pillars of Object-Oriented Design (OOD)**, and they help make code easier to write and understand.

<br>

## **🏛️ The Four Pillars of OOD 🏛️**

### 1. **Encapsulation 🔒**: Keeping Things Safe 

**Encapsulation** is like having a box where the important things are hidden away. You don’t let anyone touch the important stuff directly, only through safe methods.

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

<br>

### 2. **Abstraction 🌫️**: Hiding the Complicated Stuff 
**Abstraction** means you don’t need to know the complicated details. You just use what you need.

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

<br>

### 3. **Inheritance 🔁**: Sharing Features  
**Inheritance** is like a family where children get traits from their parents. You don’t need to create everything from scratch!

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

<br>

### 4. **Polymorphism ⚙️**: One Name, Many Actions  
**Polymorphism** means that one name can do different things! The same action can be done in different ways by different objects.

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
