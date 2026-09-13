# Student Management REST API

A beginner-friendly Java backend project for learning Spring Boot, REST APIs, layered architecture, and CRUD operations.

## What students will learn

1. Spring Boot project structure
2. REST API and HTTP methods
3. Controller → Service → Repository flow
4. Entity and JPA basics
5. CRUD operations
6. H2 database for easy local practice
7. Maven and application configuration

## Tech Stack

- Java 17+
- Spring Boot 3.x
- Spring Web
- Spring Data JPA
- H2 Database
- Maven

## Run

```bash
mvn spring-boot:run
```

The API runs on `http://localhost:8080`.

## API Endpoints

| Method | Endpoint | Purpose |
|---|---|---|
| GET | `/api/students` | Get all students |
| GET | `/api/students/{id}` | Get one student |
| POST | `/api/students` | Add a student |
| PUT | `/api/students/{id}` | Update a student |
| DELETE | `/api/students/{id}` | Delete a student |

## Sample JSON

```json
{
  "name": "Rahul",
  "email": "rahul@example.com",
  "course": "Java Backend"
}
```

## Teaching Flow

**Concept → Syntax → Example → Practice → Assignment**

### Practice

- Add 3 students.
- Fetch all students.
- Fetch a student by ID.
- Update a student's course.
- Delete a student.

### Assignment

Add validation for required fields and create a search endpoint by course.

## Project Structure

```text
student-management-api/
├── pom.xml
└── src/main/
    ├── java/com/example/studentmanagement/
    │   ├── StudentManagementApplication.java
    │   ├── controller/StudentController.java
    │   ├── entity/Student.java
    │   ├── repository/StudentRepository.java
    │   └── service/StudentService.java
    └── resources/application.properties
```
