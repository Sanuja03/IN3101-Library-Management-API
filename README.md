# Library Management REST API

A RESTful Library Management API developed for **IN3101 – Enterprise Application Development** at the University of Moratuwa.

The application allows users to manage books through REST API endpoints, using Spring Boot and MySQL.

## Technologies Used

- Java 21
- Spring Boot
- Spring Data JPA
- MySQL
- Maven
- Postman
- Swagger UI / OpenAPI

## Features

- Create a new book
- Retrieve all books
- Retrieve a book by ID
- Update book details
- Delete a book
- Input validation and appropriate HTTP status codes
- API documentation through Swagger UI

## Database Configuration

1. Create a MySQL database named `library_db`.
2. Configure the database connection in `src/main/resources/application.properties`.
3. Set the `LIBRARY_DB_PASSWORD` environment variable to your MySQL password.

## Running the Application

Make sure Java 21 and MySQL are installed and running.

On Windows, open a terminal in the project directory and execute:

```powershell
.\mvnw.cmd spring-boot:run
```

The application will run at: http://localhost:8080

## API Endpoints
| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/books` | Create a book |
| GET | `/api/books` | Retrieve all books |
| GET | `/api/books/{id}` | Retrieve a book |
| PUT | `/api/books/{id}` | Update a book |
| DELETE | `/api/books/{id}` | Delete a book |

## API Documentation
Swagger UI: http://localhost:8080/swagger-ui/index.html
