# Lesson 14 — File Handling & I/O

## Learning objectives
Read, write, copy and inspect files using modern Java I/O APIs.

## Path
```java
Path path = Path.of("notes.txt");
```

## Write and read
```java
Files.writeString(path, "Hello Java");
String text = Files.readString(path);
System.out.println(text);
```

## Lines
```java
List<String> lines = Files.readAllLines(path);
for (String line : lines) System.out.println(line);
```

For large files, prefer streaming APIs rather than loading everything into memory.

## Buffered I/O
`BufferedReader` and `BufferedWriter` are useful for efficient character I/O and controlled processing.

## Exceptions
File operations commonly involve `IOException`, so learn `try-catch` and try-with-resources.

```java
try (BufferedReader reader = Files.newBufferedReader(path)) {
    String line;
    while ((line = reader.readLine()) != null) {
        System.out.println(line);
    }
}
```

## Practice
1. Create a text file.
2. Write student records.
3. Read and count lines.
4. Search for a word in a file.
5. Copy a file.
6. Append a new record.

## Mini assignment
Create a **Notes Manager** that can create, append, read, search and delete note files safely.
