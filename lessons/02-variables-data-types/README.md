# Lesson 2 — Variables, Data Types & Type Casting

## Learning objectives
Understand variables, primitive types, reference types, literals, constants and type conversion.

## Variables
A variable is a named storage location used to hold a value.

```java
int age = 20;
double price = 99.50;
String name = "Swaraj";
```

## Primitive data types
Java has 8 primitive types:

| Type | Typical use |
|---|---|
| byte | very small integers |
| short | small integers |
| int | general integers |
| long | large integers |
| float | decimal values with lower precision |
| double | decimal values with higher precision |
| char | one UTF-16 code unit |
| boolean | true/false |

```java
int marks = 95;
double percentage = 91.5;
char grade = 'A';
boolean passed = true;
long population = 8000000000L;
```

## Reference types
Classes, arrays, interfaces, enums and other object types are reference types.

```java
String city = "Ahmedabad";
int[] numbers = {10, 20, 30};
```

## Constants
Use `final` when a variable should not be reassigned.

```java
final double PI = 3.141592653589793;
```

## Type casting
### Widening
Smaller compatible numeric types can be converted automatically.
```java
int x = 10;
double y = x;
```

### Narrowing
Explicit casting may lose information.
```java
double price = 99.99;
int whole = (int) price;
```

## String vs char
```java
char letter = 'A';
String word = "Java";
```
Use single quotes for a `char` literal and double quotes for a `String` literal.

## Common mistakes
- Using `int` when the value may exceed its range.
- Forgetting `L` for large `long` literals when needed.
- Expecting `(int) 9.9` to round; it truncates toward zero.
- Confusing `char` with `String`.

## Practice
1. Declare one variable of each primitive type.
2. Store a student's name, age, marks and pass status.
3. Demonstrate widening from `int` to `double`.
4. Demonstrate narrowing from `double` to `int`.
5. Predict the result of `(int) 15.99` before running it.

## Mini assignment
Create `StudentProfile.java` with variables for name, age, roll number, percentage, grade and pass status. Print a formatted profile.
