# 05 - JPA and H2 Database

## Concept

JPA Java objects ko relational database tables ke saath map karne me help karta hai.

`Student` class database me `students` table ko represent karti hai.

## Entity syntax

```java
@Entity
@Table(name = "students")
public class Student {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
}
```

`@Id` primary key batata hai. `@GeneratedValue` ID generate karne me help karta hai.

## Repository

```java
public interface StudentRepository extends JpaRepository<Student, Long> {
}
```

Isse save, findAll, findById aur deleteById jaise common operations mil jate hain.

## H2

H2 ek lightweight database hai jo learning ke liye convenient hai.

Console:

```text
http://localhost:8080/h2-console
```

JDBC URL:

```text
jdbc:h2:mem:studentdb
```

## Practice

H2 console me `students` table dekho aur sample records identify karo.

## Assignment

H2 ki jagah MySQL/PostgreSQL use karne ke liye required configuration research karo.
