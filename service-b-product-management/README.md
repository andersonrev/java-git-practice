# Product Management Service

This is the Product Management microservice, which provides RESTful endpoints for managing products.

## Endpoints

- **GET /productos**: Retrieve a list of all products.
- **GET /productos/{id}**: Retrieve a specific product by ID.
- **POST /productos**: Create a new product.
- **PUT /productos/{id}**: Update an existing product by ID.
- **DELETE /productos/{id}**: Delete a product by ID.

## Setup Instructions

1. Ensure you have Java and Maven installed on your machine.
2. Clone the repository:
   ```
   git clone <repository-url>
   ```
3. Navigate to the `service-b-product-management` directory:
   ```
   cd service-b-product-management
   ```
4. Build the project using Maven:
   ```
   mvn clean install
   ```
5. Run the application:
   ```
   mvn spring-boot:run
   ```

## Testing

You can test the endpoints using Postman or curl. Here are some examples:

- **Get all products**:
  ```
  curl -X GET http://localhost:8081/productos
  ```

- **Create a new product**:
  ```
  curl -X POST http://localhost:8081/productos -H "Content-Type: application/json" -d '{"name": "Product1", "price": 100}'
  ```

- **Update a product**:
  ```
  curl -X PUT http://localhost:8081/productos/1 -H "Content-Type: application/json" -d '{"name": "Updated Product", "price": 150}'
  ```

- **Delete a product**:
  ```
  curl -X DELETE http://localhost:8081/productos/1
  ```

## Configuration

The application properties can be found in `src/main/resources/application.properties`. You can configure the server port and other settings there.

## License

This project is licensed under the MIT License.