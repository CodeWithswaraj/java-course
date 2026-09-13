# Lesson 1 — Introduction to Java

## Learning objectives
By the end of this lesson, students can explain what Java is, where it is used, and why Java is popular.

## 1. What is Java?
Java is a high-level, general-purpose, object-oriented programming language designed to be portable across operating systems. Java source code is compiled into bytecode, which runs on the Java Virtual Machine (JVM).

A simple mental model:

`Java source code → compiler → bytecode → JVM → machine-specific execution`

## 2. Why learn Java?
- Readable syntax and strong tooling.
- Object-oriented programming support.
- Automatic memory management through garbage collection.
- Large standard library and ecosystem.
- Commonly used for backend services, enterprise software, Android history/legacy codebases, desktop tools and education.

## 3. Java editions
- **Java SE** — core language and standard APIs.
- **Jakarta EE** — enterprise application technologies built around Java standards.
- **Java ME** — Java technologies for constrained devices; less central to modern beginner learning.

## 4. JDK, JRE and JVM
**JVM:** Executes Java bytecode.

**JRE:** Runtime components needed to run Java applications; conceptually includes a JVM plus runtime libraries.

**JDK:** Development kit used to develop Java programs; includes tools such as the Java compiler (`javac`) and launcher (`java`).

For teaching and development, install a current JDK.

## 5. First Java program
```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, Java!");
    }
}
```

### Understand every line
- `public class HelloWorld` declares a class named `HelloWorld`.
- `main` is the standard entry point used by the Java launcher.
- `String[] args` receives command-line arguments.
- `System.out.println(...)` prints a line to standard output.
- `{}` define blocks.
- `;` ends a statement.

## 6. Compile and run
Save the file as `HelloWorld.java`.

```bash
javac HelloWorld.java
java HelloWorld
```

Expected output:
```text
Hello, Java!
```

## 7. Comments
```java
// Single-line comment

/*
   Multi-line comment
*/
```

Comments help humans understand code and are ignored by the compiler as program instructions.

## Common mistakes
1. Saving `public class HelloWorld` in a differently named file.
2. Forgetting the semicolon after a statement.
3. Running `java HelloWorld.java` when intentionally practicing the separate compile/run workflow.
4. Using `Java` when referring to the language and assuming it is the same thing as the JVM.

## Practice questions
1. What is Java bytecode?
2. What is the role of the JVM?
3. What is the difference between JDK and JVM?
4. Why does the file name normally match a public class name?
5. Write a program that prints your name, city and a favorite programming topic on separate lines.
6. Compile and run the program from the command line.

## Mini assignment
Create `AboutMe.java` that prints five facts about yourself, one per line. Do not use variables yet; focus only on class structure and output.

## Teacher tip
Have the student predict the output before running every example. Then ask them to change one line and observe what changes.