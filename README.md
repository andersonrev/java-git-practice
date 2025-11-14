# Java Microservices Application

This project consists of two microservices built with Spring Boot:

1. **Service A: User Management**
   - Manages user-related operations.
   - Exposes REST endpoints under `/usuarios`.

2. **Service B: Product Management**
   - Manages product-related operations.
   - Exposes REST endpoints under `/productos`.

## Project Structure

```
java-microservices-app
├── service-a-user-management
│   ├── src
│   │   └── main
│   │       ├── java
│   │       │   └── com
│   │       │       └── example
│   │       │           └── usermanagement
│   │       │               ├── UserManagementApplication.java
│   │       │               └── controller
│   │       │                   └── UsuarioController.java
│   │       └── resources
│   │           └── application.properties
│   ├── pom.xml
│   └── README.md
├── service-b-product-management
│   ├── src
│   │   └── main
│   │       ├── java
│   │       │   └── com
│   │       │       └── example
│   │       │           └── productmanagement
│   │       │               ├── ProductManagementApplication.java
│   │       │               └── controller
│   │       │                   └── ProductoController.java
│   │       └── resources
│   │           └── application.properties
│   ├── pom.xml
│   └── README.md
└── README.md
```

## Getting Started

### Prerequisites

- Java 11 or higher
- Maven

### Running the Microservices

1. **User Management Service**
   - Navigate to the `service-a-user-management` directory.
   - Run the following command to start the service:
     ```
     mvn spring-boot:run
     ```
   - The service will run on port `8080` by default.

2. **Product Management Service**
   - Navigate to the `service-b-product-management` directory.
   - Run the following command to start the service:
     ```
     mvn spring-boot:run
     ```
   - The service will run on port `8081` by default.

### Testing the Endpoints

You can test the endpoints using Postman or curl.

- **User Management Endpoints**
  - GET: `http://localhost:8080/usuarios`
  - POST: `http://localhost:8080/usuarios`
  - PUT: `http://localhost:8080/usuarios/{id}`
  - DELETE: `http://localhost:8080/usuarios/{id}`

- **Product Management Endpoints**
  - GET: `http://localhost:8081/productos`
  - POST: `http://localhost:8081/productos`
  - PUT: `http://localhost:8081/productos/{id}`
  - DELETE: `http://localhost:8081/productos/{id}`

## Conclusion

This project demonstrates a simple setup of microservices using Spring Boot. You can extend the functionality by adding more features and endpoints as needed.