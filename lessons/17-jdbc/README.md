# Lesson 17 — JDBC & Database Basics

## Learning objectives
Connect Java applications to relational databases and execute SQL safely.

## JDBC flow
1. Add the appropriate JDBC driver to the project.
2. Open a database connection.
3. Create a `PreparedStatement`.
4. Bind parameters.
5. Execute the statement.
6. Process the `ResultSet` when reading.
7. Close resources with try-with-resources.

## Example
```java
String sql = "SELECT id, name FROM students WHERE marks >= ?";
try (Connection connection = DriverManager.getConnection(url, user, password);
     PreparedStatement ps = connection.prepareStatement(sql)) {
    ps.setInt(1, 40);
    try (ResultSet rs = ps.executeQuery()) {
        while (rs.next()) {
            System.out.println(rs.getInt("id") + " " + rs.getString("name"));
        }
    }
}
```

## Why PreparedStatement?
It separates SQL structure from parameter values and is the standard choice for parameterized queries, helping prevent SQL injection.

## CRUD
- Create → `INSERT`
- Read → `SELECT`
- Update → `UPDATE`
- Delete → `DELETE`

## Transactions
Understand `commit`, `rollback` and transaction boundaries when multiple database changes must succeed or fail together.

## Practice
1. Connect to a database.
2. Create a students table.
3. Insert records.
4. Query records.
5. Update a student's marks.
6. Delete a student.
7. Implement a transaction.

## Mini project
Build a **JDBC Student Management System** with add, list, search, update and delete operations.
