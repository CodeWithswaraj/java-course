# Lesson 7 — Arrays

## Learning objectives
Store multiple values of the same type and process them with loops.

## Creating arrays
```java
int[] marks = {80, 92, 75, 88};
int[] numbers = new int[5];
numbers[0] = 10;
```

Indexes start at `0`.

## Traversal
```java
for (int i = 0; i < marks.length; i++) {
    System.out.println(marks[i]);
}

for (int mark : marks) {
    System.out.println(mark);
}
```

## Common operations
Find sum, average, minimum, maximum, search for an element and count occurrences.

## 2D arrays
```java
int[][] matrix = {
    {1, 2, 3},
    {4, 5, 6}
};
System.out.println(matrix[1][2]);
```

## Common mistakes
- Accessing an invalid index.
- Using `i <= array.length` instead of `i < array.length`.
- Confusing array length with the last index.

## Practice
1. Find sum and average.
2. Find min/max.
3. Reverse an array.
4. Search for a value.
5. Count duplicates.
6. Find the second-largest value.
7. Merge two arrays.
8. Add two matrices.

## Mini assignment
Create `StudentMarks.java` that stores marks for a class and prints total, average, highest, lowest, pass count and failed subjects.
