# Lesson 3 — JDK Tools and Development Workflow

## Learning objectives
Learn the basic JDK commands and a simple edit → compile → run → test workflow.

## Important commands
Check the Java launcher:
```bash
java --version
```

Check the compiler:
```bash
javac --version
```

Compile:
```bash
javac HelloWorld.java
```

Run a compiled class:
```bash
java HelloWorld
```

## Source file vs class file
`HelloWorld.java` is human-readable source code. Compilation produces bytecode, commonly stored in `HelloWorld.class` for a simple compilation.

The JVM executes bytecode; it does not directly execute the Java source text in the traditional compile/run workflow.

## A good beginner workflow
1. Create a folder for the lesson.
2. Write one small program.
3. Compile it.
4. Read compiler errors carefully if compilation fails.
5. Run it.
6. Test expected and unexpected inputs when the program accepts input.
7. Refactor only after the behavior is correct.

## Compiler errors vs runtime errors
**Compile-time error:** The source cannot be compiled, often because of invalid syntax or type rules.

**Runtime error:** The program compiled but fails while executing, such as an exception caused by invalid input or an illegal operation.

Example compile-time mistake:
```java
int age = "twenty";
```

The value is a `String`, while the variable expects an `int`.

## Command-line arguments
```java
public class ArgsDemo {
    public static void main(String[] args) {
        System.out.println("Arguments: " + args.length);
        if (args.length > 0) {
            System.out.println("First: " + args[0]);
        }
    }
}
```

Run:
```bash
javac ArgsDemo.java
java ArgsDemo Java Student
```

## Practice
1. Check your installed JDK version.
2. Compile and run `HelloWorld.java`.
3. Intentionally remove a semicolon and read the compiler message.
4. Restore the code and run it again.
5. Create a program that prints the number of command-line arguments.

## Mini assignment
Create `Greeting.java` that accepts a name as the first command-line argument and prints a greeting. If no argument is supplied, print a helpful usage message instead of accessing `args[0]` blindly.
