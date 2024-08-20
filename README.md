Forum API Gateway

Overview

The Forum API Gateway is a centralized service in the Online Forum project that manages the routing and communication between various microservices, such as user authentication, forum posts, comments, categories, and tags. It serves as the single entry point for all client requests, ensuring a streamlined and secure interaction with the underlying services. The API Gateway is designed to handle Cross-Origin Resource Sharing (t) requests and includes built-in Swagger documentation for easy API exploration and testing.

What Does It Do?

Routing: Manages and routes incoming HTTP requests to the appropriate microservices.
Security: Handles authentication via JWT (JSON Web Tokens) to secure endpoints.
CORS Management: Allows for flexible and secure cross-origin requests.
Documentation: Provides interactive API documentation through Swagger UI.
Technologies Used

**G -- Fast, unopinionated, minimalist web framework for Go.
Swagger: Provides tools to generate and serve API documentation.
Docker: Containerizes the application for consistent deployment across different environments.
CORS Middleware: Manages and configures cross-origin resource sharing policies.

How to Run the Application

Prerequisites
Docker: Ensure Docker is installed on your system.
Go: Needed if running the application locally without Docker.
Git: For cloning the repository.
Running with Docker
Clone the Repository:
bash
Copy code
git clone https://github.com/saidburkhanmukhtorov/forum-project
Build the Docker Image:
Build Docker images for every services
bash
Copy code
go run main.go
Access the Application:
API Gateway: http://localhost:8080
Swagger UI: http://localhost:8080/api/swagger/index.html
Testing

Unit Tests: Run the unit tests using the following command:
bash
Copy code
go test ./...
API Testing: You can test the API endpoints using the Swagger UI provided at http://localhost:8080/api/swagger/index.html.
Contributing

We welcome contributions! Please follow these steps to contribute:

Fork the repository.
Create a new branch (git checkout -b feature-branch).
Make your changes.
Commit your changes (git commit -m 'Add some feature').
Push to the branch (git push origin feature-branch).
Open a pull request.
License

This README file provides a comprehensive guide to understanding, deploying, and contributing to the Forum API Gateway project, ensuring that other developers can easily get started and participate in its development.
