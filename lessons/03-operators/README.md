# Lesson 3 — Operators

## Learning objectives
Learn arithmetic, assignment, relational, logical, unary, ternary and bitwise operators.

## Arithmetic
`+  -  *  /  %`

```java
int a = 17;
int b = 5;
System.out.println(a + b);
System.out.println(a / b); // integer division
System.out.println(a % b); // remainder
```

## Assignment
`=`, `+=`, `-=`, `*=`, `/=`, `%=`

```java
int score = 10;
score += 5;
```

## Relational
`==`, `!=`, `>`, `<`, `>=`, `<=` produce boolean results.

## Logical
`&&` AND, `||` OR, `!` NOT.

```java
int age = 20;
boolean eligible = age >= 18 && age <= 60;
```

Java's `&&` and `||` use short-circuit evaluation.

## Increment and decrement
```java
int x = 5;
System.out.println(x++); // 5, then x becomes 6
System.out.println(++x); // increment first, then print
```

## Ternary operator
```java
int marks = 72;
String result = marks >= 40 ? "Pass" : "Fail";
```

## Operator precedence
Use parentheses when the intended order is important.
```java
int result = (10 + 5) * 2;
```

## Bitwise operators
`&`, `|`, `^`, `~`, `<<`, `>>`, `>>>` operate at the bit level and are useful later in DSA and systems-oriented work.

## Common mistakes
- Using `=` instead of `==` in a comparison.
- Forgetting integer division: `5 / 2` is `2`.
- Confusing `x++` with `++x`.
- Writing complicated expressions without parentheses.

## Practice
1. Build a calculator for two integers.
2. Check whether a number is even using `%`.
3. Check whether a student passes using `&&`.
4. Use the ternary operator to find the larger of two numbers.
5. Predict five expressions before executing them.

## Mini assignment
Create `MarksCalculator.java` that calculates total, average, pass/fail and grade using operators.
