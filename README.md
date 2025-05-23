<img width="1236" alt="Screenshot 2025-05-16 at 5 57 02 PM" src="https://github.com/user-attachments/assets/4cd3f476-b662-4dd8-94e2-4abbc3d2b639" />
Project Title
Library Management System API

Project Description
A Library Management System API built using Spring Boot that allows librarians to manage books, patrons, and borrowing records. The system supports CRUD operations for books and patrons, manages borrowing records, and includes features for validation, error handling, optional security, caching, transaction management, and testing.

Technologies Used
Spring Boot: For creating the RESTful API and managing the application’s configuration and services.
Spring Data JPA: For database interactions and ORM (Object-Relational Mapping).
Spring Security (Optional): For implementing basic authentication or JWT-based authorization.
Spring Caching (Optional): For improving performance through caching.
Aspect-Oriented Programming (AOP) (Optional): For logging and performance monitoring.
JUnit & Mockito: For unit and integration testing of services, controllers, and repositories.
MySQL: For data storage
ModelMapper: For mapping between DTOs and entities.
Lombok: For reducing boilerplate code with annotations like @RequiredArgsConstructor and @Slf4j.


Navigate to the Project Directory: cd library-management-system
Run the Application:
Using Maven: ./mvnw spring-boot:run (or mvn spring-boot:run if Maven is installed globally)

API Endpoints
Book Management:


GET /api/books
GET /api/books/{id}
POST /api/books
PUT /api/books/{id}
DELETE /api/books/{id}
Patron Management:

GET /api/patrons
GET /api/patrons/{id}
POST /api/patrons
PUT /api/patrons/{id}
DELETE /api/patrons/{id}
Borrowing Records:

POST /api/borrow/{bookId}/patron/{patronId}
PUT /api/return/{bookId}/patron/{patronId}
Testing
Unit Tests: Located in the src/test/java directory, covering services, controllers, and repositories.
Integration Tests: Ensure API endpoints and interactions work as expected.
