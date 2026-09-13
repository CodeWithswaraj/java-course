# Lesson 13 — Generics

## Learning objectives
Write reusable, type-safe classes and methods.

## Generic class
```java
class Box<T> {
    private T value;
    void set(T value) { this.value = value; }
    T get() { return value; }
}

Box<String> box = new Box<>();
box.set("Java");
```

## Generic method
```java
static <T> void print(T value) {
    System.out.println(value);
}
```

## Bounded type parameters
```java
static <T extends Number> double square(T value) {
    double n = value.doubleValue();
    return n * n;
}
```

## Wildcards
- `?` unknown type.
- `? extends T` useful when reading from a producer.
- `? super T` useful when writing into a consumer.

A common memory aid is **PECS: Producer Extends, Consumer Super**.

## Practice
1. Create a generic `Pair<A,B>`.
2. Create a generic stack.
3. Write a bounded numeric method.
4. Use `List<? extends Number>`.
5. Explain why raw types reduce type safety.

## Mini assignment
Build a generic `Repository<T>` abstraction with add, find and remove operations.
