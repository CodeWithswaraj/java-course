# Lesson 6 — Loops

## Learning objectives
Repeat work using `for`, `while`, `do-while`, nested loops, `break` and `continue`.

## for loop
```java
for (int i = 1; i <= 5; i++) {
    System.out.println(i);
}
```

## while loop
```java
int i = 1;
while (i <= 5) {
    System.out.println(i);
    i++;
}
```

## do-while
Runs the body at least once.
```java
int choice = 0;
do {
    System.out.println("Menu");
} while (choice != 0);
```

## break and continue
`break` exits the loop. `continue` skips the rest of the current iteration.

## Nested loops and patterns
```java
for (int row = 1; row <= 3; row++) {
    for (int col = 1; col <= 4; col++) {
        System.out.print("* ");
    }
    System.out.println();
}
```

## Practice
1. Print 1 to 100.
2. Print even numbers.
3. Find the sum from 1 to N.
4. Create multiplication tables.
5. Reverse a number.
6. Check palindrome numbers.
7. Find factorial.
8. Print star and number patterns.
9. Generate Fibonacci terms.
10. Check whether a number is prime.

## Mini assignment
Create `NumberAnalyzer.java` that reads a number and reports digit count, digit sum, reverse, palindrome status and whether it is prime.
