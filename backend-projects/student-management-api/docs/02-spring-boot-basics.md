# 02 - Spring Boot Basics

## Concept

Spring Boot Java applications ko quickly create aur run karne ke liye framework hai. Ye configuration aur dependency setup ko simple banata hai.

## Maven

`pom.xml` project ki dependencies aur build configuration define karta hai.

Important dependencies:
- Spring Web
- Spring Data JPA
- H2
- Spring Boot Test

## Main class

```java
@SpringBootApplication
public class StudentManagementApplication {
    public static void main(String[] args) {
        SpringApplication.run(StudentManagementApplication.class, args);
    }
}
```

## Practice

1. `pom.xml` open karo.
2. Har dependency ka purpose identify karo.
3. Application run karo.

## Assignment

Explain karo ki `SpringApplication.run()` kya karta hai aur `@SpringBootApplication` ka purpose kya hai.
