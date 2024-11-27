# Node Docker Project

This project demonstrates the integration of the Fastify framework into a Node.js application, utilizing Docker Compose for containerized deployment. The application includes RESTful endpoints and is configured to work seamlessly with Nginx.

## Project Overview

### 1. Node.js Basics
- Reviewed the fundamentals of Node.js.
- Revisited concepts of asynchronous programming and event-driven architecture in Node.js.

### 2. Introduction to Fastify
- Explored Fastify framework and its core features, such as high performance and ease of use.
- Learned the basic syntax for:
  - Setting up a Fastify server.
  - Configuring routes.
  - Handling requests.

### 3. Integrating Fastify with Docker Compose
- Replaced the existing framework (e.g., Express) with Fastify in the project.
- Configured Fastify to handle basic RESTful routes, including:
  - Create (POST)
  - Read (GET)
  - Update (PUT)
  - Delete (DELETE)
- Updated `Dockerfile` and `docker-compose.yml` to set Fastify as the primary server framework.

### 4. Implementing RESTful Endpoints
Implemented the following endpoints:

- **GET /api/resources**: Retrieve a list of all resources.
- **GET /api/resources/:id**: Retrieve a resource by ID.
- **POST /api/resources**: Create a new resource.
- **PUT /api/resources/:id**: Update an existing resource by ID.
- **DELETE /api/resources/:id**: Delete a resource by ID.

Each endpoint includes basic validation for incoming request data.

### 5. Configuring Fastify with Nginx
- Configured Fastify to function correctly behind the Nginx proxy server.
- Ensured compatibility with Nginx features such as:
  - Static file serving.
  - Proxying API requests.

### 6. Deployment and Testing
- Deployed the updated project using Docker Compose.
- Tested the application to ensure:
  - All RESTful endpoints work as expected.
  - The system handles requests efficiently.
  - Integration with Nginx operates correctly.

## Getting Started

### Prerequisites
- Node.js (v14 or higher recommended)
- Docker and Docker Compose
- Basic knowledge of RESTful APIs

### Testing
You can test the RESTful endpoints using tools like Postman or curl. Ensure all expected responses and behaviors are verified.

## Future Enhancements
- Add authentication and authorization mechanisms.
- Integrate database support (e.g., MongoDB, PostgreSQL).
- Enhance validation with schemas and middleware.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.
```