# 🚀 **Object-Oriented Design (OOD) Basics**

### **What is Object-Oriented Design?**
Object-Oriented Design (OOD) is a way of organizing your code. Instead of everything being a big mess, you group related things together into **objects**. Each object has **data** (like a name or number) and **actions** (like moving or changing).

<br>

### **The Four Pillars of OOD**

#### **1. Encapsulation: Keeping Things Safe**
Encapsulation is like having a box where the important things are hidden away. You don’t let anyone touch the important stuff directly, only through safe methods.

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
