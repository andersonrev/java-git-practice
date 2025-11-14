# User Management Service

## Overview
This project contains the User Management microservice, which provides RESTful endpoints for managing users. It is part of a larger application that includes a Product Management microservice.

## Technologies Used
- Java
- Spring Boot
- Maven

## Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone <repository-url>
   cd java-microservices-app/service-a-user-management
   ```

2. **Build the Project**
   Ensure you have Maven installed. Run the following command to build the project:
   ```bash
   mvn clean install
   ```

3. **Run the Application**
   You can run the application using the following command:
   ```bash
   mvn spring-boot:run
   ```

   By default, the service will run on port `8080`. You can change this in the `src/main/resources/application.properties` file.

## Endpoints

- **GET /usuarios**
  - Retrieves a list of users.

- **POST /usuarios**
  - Creates a new user.

- **PUT /usuarios/{id}**
  - Updates an existing user by ID.

- **DELETE /usuarios/{id}**
  - Deletes a user by ID.

## Testing the Endpoints
You can test the endpoints using Postman or curl.

### Example using curl:
- **Get all users**
  ```bash
  curl -X GET http://localhost:8080/usuarios
  ```

- **Create a new user**
  ```bash
  curl -X POST http://localhost:8080/usuarios -H "Content-Type: application/json" -d '{"name": "John Doe", "email": "john@example.com"}'
  ```

## Additional Information
For more details on the Product Management microservice, please refer to the `service-b-product-management/README.md` file.