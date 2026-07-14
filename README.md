# Expense Tracker

An expense-tracking application backend built with **Java** and **Spring Boot**, developed as part of a professional practice project and following industry best practices in backend development.

## Overview

This project implements the backend of an expense tracker application. It allows users to manage their personal expenses through a secure, well-documented RESTful API, while demonstrating best practices in authentication, asynchronous messaging, testing, and containerized deployment.

## Features

- RESTful API for managing expenses (create, read, update, delete)
- Secure authentication and authorization with **Spring Security**
- Asynchronous message processing using **RabbitMQ**
- Interactive API documentation via **Swagger / OpenAPI**
- Unit and integration testing with **JUnit**
- Containerized setup with **Docker** for consistent deployment

> Note: Update this section with the exact business features of your app (e.g. expense categories, budgets, reports, currency support) if they differ from the above.

## Tech Stack

| Category         | Technology            |
|-------------------|------------------------|
| Language          | Java                  |
| Framework         | Spring Boot           |
| Security          | Spring Security        |
| Messaging         | RabbitMQ               |
| Testing           | JUnit                  |
| API Documentation | Swagger / OpenAPI      |
| Containerization  | Docker                 |
| Build Tool        | Maven                  |

## Prerequisites

Before running this project locally, make sure you have the following installed:

- Java JDK 17+ (adjust to the version used in your project)
- Maven
- Docker (optional, for containerized run)
- RabbitMQ (running locally or via Docker)

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/AnicaDjukic/Expense-Tracker.git
cd Expense-Tracker
```

### 2. Build the project

```bash
mvn clean install
```

### 3. Run the application

```bash
mvn spring-boot:run
```

By default, the application runs on:

```
http://localhost:8080
```

### 4. Run with Docker (optional)

```bash
docker build -t expense-tracker .
docker run -p 8080:8080 expense-tracker
```

> Adjust the Dockerfile/image name and port mapping if they differ from the ones used in the actual project.

## API Documentation

Once the application is running, the API documentation is available via Swagger UI:

```
http://localhost:8080/swagger-ui.html
```

## Testing

Run unit and integration tests with:

```bash
mvn test
```

## Project Structure

```
Expense-Tracker/
├── ExpenseTracker/                     # Main application source code
├── expense_tracker.postman_collection  # Postman collection for API testing
├── rabbitMqMessages.txt                # Sample RabbitMQ message formats
└── README.md
```


**Anica Djukic**
GitHub: [@AnicaDjukic](https://github.com/AnicaDjukic)

## License

This project currently has no license specified. Add a `LICENSE` file if you'd like to make usage terms explicit (e.g. MIT, Apache 2.0).