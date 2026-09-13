# Lesson 2 — Java Program Structure

## Learning objectives
Understand classes, methods, blocks, statements, identifiers and the `main` method.

## Basic structure
```java
public class StudentApp {
    public static void main(String[] args) {
        System.out.println("Student app started");
    }
}
```

## Class
A class is a blueprint/type definition. It can contain fields, constructors, methods and nested types.

```java
class Calculator {
    int add(int a, int b) {
        return a + b;
    }
}
```

## Method
A method groups behavior that can be called by name.

```java
static void greet() {
    System.out.println("Welcome");
}
```

`static` means the method belongs to the class rather than requiring an instance for this call.

## Statements and blocks
```java
int age = 20;
System.out.println(age);
```

Statements usually end with `;`. Curly braces create blocks such as class, method and conditional blocks.

## Identifiers
Identifiers are names for classes, methods, variables and other program elements.

Good examples:
```text
Student
calculateTotal
studentCount
MAX_SIZE
```

Avoid confusing names such as `x1x2x3` when a descriptive name is possible.

## Naming conventions
- Classes: `PascalCase` — `StudentManager`
- Methods/variables: `camelCase` — `calculateMarks`
- Constants: `UPPER_SNAKE_CASE` — `MAX_RETRY_COUNT`
- Packages: lowercase — `com.example.school`

## `main` method
The common entry-point declaration is:
```java
public static void main(String[] args)
```

The Java launcher looks for this compatible entry point when starting a traditional application class.

## Escape sequences
```java
System.out.println("Hello\nWorld");
System.out.println("Name:\tSwaraj");
System.out.println("He said \"Java\".");
```

## Practice
1. Identify the class, method and statements in a sample program.
2. Rename a poorly named variable using Java naming conventions.
3. Write a program with two methods and call both from `main`.
4. Print a three-line message using `\n`.
5. Print two values separated by a tab using `\t`.

## Mini assignment
Build `StudentApp.java` with a `main` method and three static methods: `showWelcome()`, `showCourse()` and `showGoal()`. Call all three from `main`.
