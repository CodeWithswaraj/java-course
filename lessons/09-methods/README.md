# Lesson 9 — Methods

## Learning objectives
Break programs into reusable methods with parameters and return values.

## Basic method
```java
static void greet(String name) {
    System.out.println("Hello " + name);
}
```

## Return values
```java
static int add(int a, int b) {
    return a + b;
}
```

## Parameters and arguments
A parameter appears in the method declaration; an argument is the value passed at the call site.

## Method overloading
Multiple methods can share a name when their parameter lists differ.
```java
static int add(int a, int b) { return a + b; }
static double add(double a, double b) { return a + b; }
```

Return type alone cannot overload a method.

## Scope
Variables declared inside a method are local to that method. Instance and class fields have different lifetimes and access patterns.

## Java is pass-by-value
Java passes values to methods. For object references, the reference value itself is copied; a method can mutate the referenced object but cannot replace the caller's reference by assigning its parameter.

## Recursion preview
A recursive method calls itself and needs a correct base case.

## Practice
1. Write methods for add/subtract/multiply/divide.
2. Write a method to test prime numbers.
3. Write a method to calculate factorial.
4. Overload a method for different numeric types.
5. Write a recursive factorial.

## Mini assignment
Create `Calculator.java` using separate methods for each operation and input validation for division by zero.
