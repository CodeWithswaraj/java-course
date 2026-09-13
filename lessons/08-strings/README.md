# Lesson 8 — Strings & StringBuilder

## Learning objectives
Understand String creation, comparison, searching, modification, immutability and efficient mutable text building.

## String basics
```java
String name = "Java";
System.out.println(name.length());
System.out.println(name.toUpperCase());
```

Strings are objects and are immutable: operations that appear to modify a String create another String value rather than changing the original object.

## Comparison
Use `.equals()` for content comparison.
```java
String a = "Java";
String b = new String("Java");
System.out.println(a.equals(b)); // true
```
Use `==` primarily for reference identity, not String content.

## Useful methods
`length()`, `charAt()`, `substring()`, `contains()`, `startsWith()`, `endsWith()`, `indexOf()`, `replace()`, `trim()`, `split()`, `toLowerCase()`, `toUpperCase()`.

## StringBuilder
For repeated modifications, `StringBuilder` is usually more suitable than repeatedly creating Strings.
```java
StringBuilder sb = new StringBuilder();
sb.append("Java");
sb.append(" Course");
sb.reverse();
System.out.println(sb);
```

## Practice
1. Reverse a string.
2. Check palindrome.
3. Count vowels/consonants.
4. Count words.
5. Find character frequency.
6. Remove spaces.
7. Check whether two strings are anagrams.

## Mini assignment
Create `TextAnalyzer.java` that reads a sentence and reports length, word count, vowel count, digit count, reversed text and palindrome status.
