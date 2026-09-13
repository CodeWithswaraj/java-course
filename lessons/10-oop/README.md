# Lesson 10 — Object-Oriented Programming

## Learning objectives
Understand classes, objects, fields, constructors, `this`, encapsulation, inheritance, polymorphism, abstraction and interfaces.

## Class and object
A class defines a type; an object is an instance of that type.
```java
class Student {
    String name;
    int age;

    Student(String name, int age) {
        this.name = name;
        this.age = age;
    }

    void introduce() {
        System.out.println("I am " + name);
    }
}

Student s = new Student("Asha", 20);
s.introduce();
```

## Encapsulation
Keep state private and expose controlled operations.
```java
class BankAccount {
    private double balance;

    public void deposit(double amount) {
        if (amount > 0) balance += amount;
    }

    public double getBalance() { return balance; }
}
```

## Inheritance
```java
class Animal {
    void sound() { System.out.println("Some sound"); }
}
class Dog extends Animal {
    @Override
    void sound() { System.out.println("Bark"); }
}
```

## Polymorphism
A parent-type reference can refer to a child object, and overridden instance methods are selected at runtime.
```java
Animal animal = new Dog();
animal.sound();
```

## `this`
Refers to the current object; commonly used to distinguish fields from parameters and to invoke another constructor.

## `super`
Used to access superclass members and constructors.

## Abstraction
Use abstract classes when you want a shared abstraction with possible state or implemented behavior.

```java
abstract class Shape {
    abstract double area();
}
```

## Interfaces
Interfaces define contracts that classes can implement.
```java
interface Payable {
    double amount();
}
```
A class can implement multiple interfaces.

## Constructor rules
Constructors initialize objects and have the same name as the class with no return type. If you declare a constructor, Java does not automatically provide a no-argument constructor for you.

## Composition
Prefer “has-a” relationships where appropriate: a `Car` can have an `Engine` object instead of inheriting from `Engine`.

## Practice
1. Create a `Student` class.
2. Create `BankAccount` with encapsulation.
3. Build `Animal`, `Dog`, `Cat` and demonstrate overriding.
4. Create an abstract `Shape` class.
5. Create an interface `PaymentMethod` and two implementations.
6. Demonstrate composition with `Car` and `Engine`.

## Mini project
Build a console-based **Library Management System** using classes such as `Book`, `Member`, `Library` and `Librarian`. Practice constructors, encapsulation, collections and polymorphism.

## Interview checkpoints
- Class vs object
- Overloading vs overriding
- Encapsulation vs abstraction
- Inheritance vs composition
- Why Java does not support multiple class inheritance
- Compile-time vs runtime polymorphism
