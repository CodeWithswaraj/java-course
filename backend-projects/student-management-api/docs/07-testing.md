# 07 - Testing

## Concept

Testing se confirm hota hai ki application expected way me kaam kar rahi hai.

Project me Spring Boot context test diya gaya hai.

## Run tests

```bash
mvn test
```

## Test example

```java
@SpringBootTest
class StudentManagementApplicationTests {
    @Test
    void contextLoads() {
    }
}
```

`@SpringBootTest` application context ko load karta hai. Agar configuration/dependencies me major problem ho to test fail ho sakta hai.

## Practice

1. `mvn test` run karo.
2. Test ka output dekho.
3. Application me intentional configuration error karke test behavior observe karo.

## Assignment

MockMvc ka use karke GET `/api/students` aur POST `/api/students` ke integration tests add karo.
