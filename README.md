# My Cool App

https://www.udemy.com/course/spring-hibernate-tutorial

This is a simple Spring Boot application that demonstrates the basic features of the Spring Boot framework.

## Features

*   **Embedded Tomcat Server:** The application runs on an embedded Tomcat server, so you don't need to deploy it to a separate web server.
*   **REST Endpoint:** The application exposes a single REST endpoint that returns a "Hello World!" message.

## Endpoints

*   `GET /`: Returns the message "Hello World!".

## Dependencies

This project uses the following dependencies:

*   **`spring-boot-starter-web`**: This is the main dependency that provides all the necessary components for building a web application with Spring Boot. It includes:
    *   An embedded Tomcat server
    *   Spring MVC for building RESTful web services
    *   Jackson for JSON serialization and deserialization

*   **`spring-boot-starter-test`**: This dependency provides all the necessary components for testing a Spring Boot application. It includes:
    *   JUnit 5 for writing unit tests
    *   Mockito for creating mock objects
    *   AssertJ for writing fluent assertions

## Continuous Integration

This project uses GitHub Actions for continuous integration. The workflow is defined in the `.github/workflows/build.yml` file and it performs the following steps:

1.  **Triggers**: The workflow is triggered on every `push` or `pull_request` to the `master` branch.
2.  **Checkout**: It checks out the source code from the repository.
3.  **Set up JDK**: It sets up a Java Development Kit (JDK) version 17.
4.  **Build with Maven**: It builds the project using Maven, creating a JAR file.

This ensures that the code is always in a buildable state.

## How to Run

1.  **Prerequisites:**
    *   Java 17 or later
    *   Maven 3.2 or later

2.  **Build the application:**
    ```bash
    mvn clean install
    ```

3.  **Run the application:**
    ```bash
    java -jar target/mycoolapp-0.0.1-SNAPSHOT.jar
    ```

4.  **Access the application:**
    Open your web browser and navigate to `http://localhost:8080`. You should see the message "Hello World!".
