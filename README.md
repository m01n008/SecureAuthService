SecureAuthService README
# SecureAuthService

A secure authentication microservice built with Spring Boot that implements JWT-based authentication with token refresh support. Designed to be containerized with Docker and integrated with a CI/CD pipeline for rapid and secure deployments.

## Features

- JWT Authentication with access and refresh tokens  
- Secure password hashing with BCrypt  
- Role-Based Access Control (RBAC) support  
- Token revocation and refresh handling  
- Dockerized for easy deployment  
- CI/CD pipeline configured with GitHub Actions  
- Protection against common security threats like token hijacking and replay attacks  

## Tech Stack

- Java 17  
- Spring Boot  
- Spring Security  
- JWT (JSON Web Tokens)  
- Docker  
- GitHub Actions (CI/CD)  

## Getting Started

### Prerequisites

- Java 17+  
- Docker  
- Maven  

### Running Locally

1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/SecureAuthService.git
   cd SecureAuthService


Build the project:

mvn clean install


Run the application:

mvn spring-boot:run

Running with Docker

Build the Docker image:

docker build -t secureauthservice .


Run the Docker container:

docker run -p 8080:8080 secureauthservice

API Endpoints

/api/auth/login - Authenticate user and issue tokens

/api/auth/refresh - Refresh access token using refresh token

/api/auth/register - Register a new user

/api/users - Secured user operations (requires authentication)

License

MIT License
