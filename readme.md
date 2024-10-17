# Simple REST Service - Spring Boot Application

This is a simple Spring Boot REST service application that demonstrates basic API functionalities such as receiving GET requests and returning JSON responses.

## Prerequisites

1. Java 11 or above
2. Maven 3.6.3 or above
3. An IDE such as IntelliJ IDEA or Visual Studio Code

## Project Structure

- **src/main/java/com/example/simplerestservice**: Contains the application logic.
  - **controller**: Houses the controller logic that handles incoming HTTP requests.
  - **model**: Contains data model classes.
  - **resources**: Configuration files such as `application.properties`.
- **src/test**: Unit test files.
- **pom.xml**: Maven configuration file.
- **README.md**: This file contains project documentation.
- **.gitignore**: Git ignore file for ignoring unnecessary files.

## How to Run the Application

1. Open a terminal and navigate to the root directory of the project.
2. Run the following command to start the application:

    ```bash
    mvn spring-boot:run
    ```

3. The application will run on port `8080` by default. Open a browser or API tool like Postman to access the endpoints.

    Example:

    ```
    http://localhost:8080/greeting?name=John
    ```

## Endpoints

- **GET /greeting**: Returns a greeting message. You can pass a query parameter `name` to personalize the greeting.
  - Example:
    
    ```bash
    curl http://localhost:8080/greeting?name=John
    ```

    Response:

    ```json
    {
      "message": "Hello, John!"
    }
    ```

## Technologies Used

- Java
- Spring Boot
- Maven
- REST API

## License

This project is licensed under the MIT License.
