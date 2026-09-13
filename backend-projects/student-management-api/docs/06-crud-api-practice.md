# 06 - CRUD API Practice

## Concept

CRUD means:

- Create
- Read
- Update
- Delete

## Create

```java
@PostMapping
public ResponseEntity<Student> create(@RequestBody Student student) {
    return ResponseEntity.ok(service.create(student));
}
```

## Read

```java
@GetMapping
public ResponseEntity<List<Student>> getAll() {
    return ResponseEntity.ok(service.getAll());
}
```

## Update

```java
@PutMapping("/{id}")
```

## Delete

```java
@DeleteMapping("/{id}")
```

## Practice sequence

1. Start application.
2. GET all students.
3. POST a new student.
4. GET the new student by ID.
5. PUT to change course.
6. GET again to verify.
7. DELETE the student.
8. GET by ID and observe the not-found behavior.

## Assignment

Add a `phone` field and update POST/PUT operations so phone is stored in the database.
