# Insurance Domain Web Application

Welcome to the Insurance Domain Web Application project. This project combines a front-end implemented with HTML, CSS, and AngularJS, and a back-end implemented using Java Spring Boot. The application is designed to provide insurance-related functionalities and can be run on port 8081.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Running the Application](#running-the-application)
- [API Endpoints](#api-endpoints)
- [Testing](#testing)
- [Documentation](#documentation)

## Prerequisites
Before running the application, make sure you have the following prerequisites installed on your system:
- Java Development Kit (JDK)
- Maven
- Node.js and npm (for AngularJS)
- Git
- An integrated development environment (IDE) for Java Spring Boot (e.g., IntelliJ IDEA or Eclipse)

## Running the Application
Follow these steps to run the Insurance Domain Web Application:

1. Clone the project repository to your local machine:


2. Front-End (HTML, CSS, AngularJS):
- Navigate to the front-end directory in your project folder.
- Install the required dependencies:

  ```
  npm install
  ```

- Start the front-end development server on port 8081:

  ```
  ng serve --port 8081
  ```

- The front-end will be accessible at http://localhost:8081 in your web browser.

3. Back-End (Java Spring Boot):
- Open the project in your Java Spring Boot-compatible IDE.
- Locate the `application.properties` or `application.yml` configuration file.
- Set the server port to 8081:

  ```
  server.port=8081
  ```

- Run the Spring Boot application from your IDE or using the command-line interface:

  ```
  mvn spring-boot:run
  ```

- The back-end API will be accessible at http://localhost:8081.

## API Endpoints
The application provides the following API endpoints:
- POST /createPolicy
- PUT /updatePolicy/{policy id}
- GET /viewPolicy/{policy id}
- DELETE /deletePolicy/{policy id}

These endpoints are used to manage insurance policies in the system.

## Testing
The project includes test suites for both the front-end and back-end components. You can run the tests to ensure the application functions correctly.

To run the tests, follow these steps:

1. For the front-end, navigate to the front-end directory and run:


2. For the back-end, use your IDE or run:


## Documentation

Feel free to explore the codebase, make improvements, and adapt it to your specific needs.

Thank you for using the Insurance Domain Web Application.
