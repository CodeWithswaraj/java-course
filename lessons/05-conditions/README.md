# Lesson 5 — Conditional Statements

## Learning objectives
Use `if`, `else if`, `else` and `switch` to make decisions.

## if / else
```java
int marks = 72;
if (marks >= 40) {
    System.out.println("Pass");
} else {
    System.out.println("Fail");
}
```

## else-if ladder
```java
if (marks >= 90) grade = 'A';
else if (marks >= 75) grade = 'B';
else if (marks >= 60) grade = 'C';
else if (marks >= 40) grade = 'D';
else grade = 'F';
```

Use braces consistently, especially while teaching beginners.

## Nested conditions
A condition can contain another condition, but avoid unnecessary nesting when a simpler expression is clearer.

## switch
```java
int day = 2;
switch (day) {
    case 1 -> System.out.println("Monday");
    case 2 -> System.out.println("Tuesday");
    default -> System.out.println("Other");
}
```

The arrow-style switch syntax is a modern form. Traditional `case:` syntax is also useful to recognize in existing code.

## Practice
1. Check positive/negative/zero.
2. Find the largest of three numbers.
3. Build a grade calculator.
4. Create a menu-driven calculator with `switch`.
5. Check leap-year rules correctly.

## Mini assignment
Build `TicketPrice.java` that calculates a ticket category or price from age and demonstrates both conditions and a switch-based menu.
