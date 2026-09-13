# Lesson 4 — Input & Output

## Learning objectives
Read user input and produce clear console output.

## Output
```java
System.out.println("Hello");
System.out.print("Java ");
System.out.printf("Marks: %d%n", 95);
```

## Scanner
```java
import java.util.Scanner;

public class InputDemo {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter your age: ");
        int age = sc.nextInt();
        System.out.println("Age = " + age);
        sc.close();
    }
}
```

Useful methods include `nextInt()`, `nextDouble()`, `next()`, `nextLine()` and `nextBoolean()`.

## The nextInt/nextLine issue
After `nextInt()`, the newline remains in the input buffer. If you immediately call `nextLine()`, consume that newline first when appropriate.

```java
int age = sc.nextInt();
sc.nextLine();
String name = sc.nextLine();
```

## Formatting
```java
String name = "Swaraj";
int marks = 88;
System.out.printf("%s scored %d%n", name, marks);
```

## Practice
1. Read name and age.
2. Read two numbers and print their sum.
3. Read three marks and calculate average.
4. Build a simple bill printer.
5. Practice both `next()` and `nextLine()`.

## Mini assignment
Create `StudentInput.java` that reads a student's name, age, three subject marks and prints a neat report card.
