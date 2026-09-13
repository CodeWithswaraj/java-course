# Lesson 11 — Exception Handling

## Learning objectives
Understand exceptions, checked vs unchecked exceptions, `try`, `catch`, `finally`, `throw` and `throws`.

## Basic handling
```java
try {
    int result = 10 / 0;
} catch (ArithmeticException e) {
    System.out.println("Cannot divide by zero");
} finally {
    System.out.println("Cleanup step");
}
```

## Common exceptions
`ArithmeticException`, `NullPointerException`, `ArrayIndexOutOfBoundsException`, `NumberFormatException`, `IllegalArgumentException`.

## Checked exceptions
Some exceptions must be handled or declared, such as many I/O exceptions.

## throw
Use `throw` to explicitly signal an exception.
```java
if (age < 0) {
    throw new IllegalArgumentException("Age cannot be negative");
}
```

## throws
A method can declare exceptions that callers must account for.

## Custom exception
```java
class InvalidMarksException extends Exception {
    InvalidMarksException(String message) { super(message); }
}
```

## Good practice
Catch specific exceptions, provide useful messages, avoid empty catch blocks, and do not use exceptions as normal control flow.

## Practice
1. Handle divide-by-zero.
2. Safely parse an integer.
3. Handle invalid array access.
4. Create a custom exception for invalid marks.
5. Write a method using `throws`.

## Mini assignment
Build `ATM.java` that validates PIN attempts, balance, withdrawal amount and insufficient funds using appropriate exceptions.
