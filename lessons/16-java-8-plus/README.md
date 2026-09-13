# Lesson 16 — Java 8+ Features

## Learning objectives
Use lambdas, functional interfaces, method references, Streams, Optional and the modern date/time API.

## Lambda
```java
List<String> names = List.of("Asha", "Ravi", "Neha");
names.forEach(name -> System.out.println(name));
```

## Functional interface
An interface with one abstract method can be used as a lambda target.
```java
@FunctionalInterface
interface Calculator {
    int apply(int a, int b);
}
```

## Method reference
```java
names.forEach(System.out::println);
```

## Stream API
```java
List<Integer> evenSquares = List.of(1, 2, 3, 4, 5, 6).stream()
    .filter(n -> n % 2 == 0)
    .map(n -> n * n)
    .toList();
```
Learn `filter`, `map`, `flatMap`, `sorted`, `distinct`, `limit`, `reduce`, `collect`, `groupingBy` and `joining`.

Streams are pipelines; intermediate operations are generally lazy, while terminal operations trigger processing.

## Optional
Use `Optional<T>` to represent a potentially absent value in APIs where it improves clarity. Do not blindly use it for every field or parameter.

## Date and time
Prefer `java.time`: `LocalDate`, `LocalTime`, `LocalDateTime`, `Instant`, `Duration`, `Period`, `ZoneId` and `DateTimeFormatter`.

## Interface default/static methods
Modern interfaces can provide `default` and `static` methods in addition to abstract methods.

## Practice
1. Convert a loop to a lambda.
2. Filter even numbers with Streams.
3. Map names to uppercase.
4. Find max/min with Streams.
5. Group objects by a property.
6. Use `Optional` safely.
7. Format a `LocalDate`.

## Mini assignment
Create a **Student Analytics** program using a `List<Student>` and Streams to calculate average marks, top students, pass count, grouping by grade and sorted reports.
