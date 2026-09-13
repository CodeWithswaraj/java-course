# 01 - Project Overview

## Concept

Backend ka kaam client ki request receive karna, business logic chalana aur database se data manage karke response dena hai.

Is project me hum Student Management API banayenge.

## Architecture

```text
Client → Controller → Service → Repository → Database
```

### Controller
HTTP request receive karta hai.

### Service
Business logic rakhta hai.

### Repository
Database operations karta hai.

### Entity
Database table ka Java representation hai.

## Syntax / Important annotations

```java
@RestController
@RequestMapping("/api/students")
```

## Example

Client `GET /api/students` bhejta hai. Controller service ko call karta hai, service repository ko call karti hai aur database se students return hote hain.

## Practice

Student se pucho: Controller aur Repository me kya difference hai?

## Assignment

Apne words me complete request flow diagram banao.
