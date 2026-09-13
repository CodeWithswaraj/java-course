# Student Management REST API

A complete beginner-friendly Java backend project for teaching **Spring Boot + REST API + JPA + H2 + Maven**.

## 1. Project Goal

We will build a Student Management REST API where a client can create, read, update, delete, and search students.

### What the student will learn

- Spring Boot application structure
- Maven and `pom.xml`
- Dependency Injection
- REST API and HTTP methods
- JSON request/response
- `@RestController`, `@RequestMapping`, `@GetMapping`, `@PostMapping`, `@PutMapping`, `@DeleteMapping`
- Controller → Service → Repository architecture
- JPA Entity and database mapping
- `JpaRepository`
- CRUD operations
- H2 database
- Query parameters and path variables
- Basic testing with Spring Boot Test
- How to read and understand a real backend project

## 2. Tech Stack

- Java 17+
- Spring Boot 3.x
- Spring Web
- Spring Data JPA
- H2 Database
- Maven
- JUnit / Spring Boot Test

## 3. Folder Structure

```text
student-management-api/
├── README.md
├── .gitignore
├── pom.xml
├── src/
│   ├── main/
│   │   ├── java/com/example/studentmanagement/
│   │   │   ├── StudentManagementApplication.java
│   │   │   ├── controller/
│   │   │   │   └── StudentController.java
│   │   │   ├── entity/
│   │   │   │   └── Student.java
│   │   │   ├── repository/
│   │   │   │   └── StudentRepository.java
│   │   │   └── service/
│   │   │       └── StudentService.java
│   │   └── resources/
│   │       ├── application.properties
│   │       └── data.sql
│   └── test/java/com/example/studentmanagement/
│       └── StudentManagementApplicationTests.java
└── docs/
    ├── 01-project-overview.md
    ├── 02-spring-boot-basics.md
    ├── 03-rest-api-and-http.md
    ├── 04-controller-service-repository.md
    ├── 05-jpa-and-h2.md
    ├── 06-crud-api-practice.md
    ├── 07-testing.md
    └── 08-practice-and-assignment.md
```

## 4. How the backend works

```text
Client / Postman
       ↓
Controller
       ↓
Service
       ↓
Repository
       ↓
H2 Database
       ↓
Repository
       ↓
Service
       ↓
Controller
       ↓
JSON Response
```

## 5. Run the project

Make sure Java 17+ and Maven are installed.

```bash
mvn spring-boot:run
```

Application URL:

```text
http://localhost:8080
```

Run tests:

```bash
mvn test
```

## 6. API Endpoints

| Method | Endpoint | Purpose |
|---|---|---|
| GET | `/api/students` | Get all students |
| GET | `/api/students/{id}` | Get one student |
| GET | `/api/students?course=Java Backend` | Search by course |
| POST | `/api/students` | Create student |
| PUT | `/api/students/{id}` | Update student |
| DELETE | `/api/students/{id}` | Delete student |

## 7. POST Example

Request:

```http
POST /api/students
Content-Type: application/json
```

```json
{
  "name": "Swaraj",
  "email": "swaraj@example.com",
  "course": "Java Backend"
}
```

## 8. PUT Example

```http
PUT /api/students/1
Content-Type: application/json
```

```json
{
  "name": "Rahul Kumar",
  "email": "rahul@example.com",
  "course": "Spring Boot"
}
```

## 9. H2 Database Console

Open:

```text
http://localhost:8080/h2-console
```

Use:

```text
JDBC URL: jdbc:h2:mem:studentdb
User Name: sa
Password: [leave empty]
```

## 10. Teaching Plan

Each lesson follows:

**Concept → Syntax → Example → Practice → Assignment**

### Lesson order

1. Project overview and backend basics
2. Spring Boot and Maven
3. REST API and HTTP methods
4. Controller, Service and Repository
5. Entity, JPA and H2
6. CRUD implementation
7. Testing
8. Practice and assignment

See the `docs/` folder for the complete lesson notes.

## 11. Practice Tasks

- Add 5 students using POST.
- Get all students.
- Get a student by ID.
- Update a student's course.
- Delete a student.
- Search students by course.
- Try an ID that does not exist and understand the error.

## 12. Student Assignment

### Beginner

1. Add a `phone` field.
2. Add an endpoint to search by name.
3. Add validation for empty name/email/course.

### Intermediate

1. Add a `department` field.
2. Add sorting by student name.
3. Add pagination.
4. Create a custom exception for student-not-found.

### Advanced

1. Add DTO classes.
2. Add global exception handling with `@ControllerAdvice`.
3. Add PostgreSQL/MySQL instead of H2.
4. Add Swagger/OpenAPI documentation.
5. Add authentication and authorization.

## 13. Important Rule for Learning

Do not only copy the code. First understand what each layer does, then type the code yourself and test every endpoint in Postman.
