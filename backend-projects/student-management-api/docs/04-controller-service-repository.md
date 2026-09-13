# 04 - Controller, Service and Repository

## Concept

Code ko layers me divide karne se project clean aur maintainable hota hai.

### Controller
Request/response handle karta hai.

### Service
Business rules aur operations handle karta hai.

### Repository
Database se baat karta hai.

## Example

```java
@RestController
@RequestMapping("/api/students")
public class StudentController {
    private final StudentService service;

    public StudentController(StudentService service) {
        this.service = service;
    }
}
```

Constructor injection se Spring `StudentService` object provide karta hai.

Repository:

```java
public interface StudentRepository extends JpaRepository<Student, Long> {
}
```

## Practice

Trace karo: `GET /api/students/1` kis-kis class se pass hota hai?

## Assignment

Controller me database code likhne ke kya disadvantages hain? Apne words me answer do.
