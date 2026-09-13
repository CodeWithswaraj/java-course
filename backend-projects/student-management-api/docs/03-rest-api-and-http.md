# 03 - REST API and HTTP

## Concept

REST API client aur server ke beech communication ka common style hai.

Common HTTP methods:

- GET → data read
- POST → new data create
- PUT → existing data update
- DELETE → data delete

## Endpoint examples

```text
GET    /api/students
GET    /api/students/1
POST   /api/students
PUT    /api/students/1
DELETE /api/students/1
```

## JSON

POST/PUT request me JSON body bhej sakte hain:

```json
{
  "name": "Rahul",
  "email": "rahul@example.com",
  "course": "Java Backend"
}
```

## Practice

Postman me GET aur POST request run karo.

## Assignment

Har HTTP method ka real-life example likho aur GET aur POST ka difference explain karo.
