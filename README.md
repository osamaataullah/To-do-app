# To-Do Application API

## Overview

This is a REST API-based To-Do application built using Java, Spring Boot, MySQL, and Spring Security. It allows users to manage tasks securely using database authentication and JWT.

## Technologies Used

- **Backend:** Java, Spring Boot, Spring Security
- **Database:** MySQL
- **Security:** Database authentication, JWT
- **Architecture:** Controller, Service, Repository Layer

## Features

- **User Management:** Role-based access (Admin, User), JWT authentication
- **To-Do Management:** Add, retrieve, update, delete To-Dos, mark as complete/incomplete

## Setup

1. **Clone the Repository:**
   ```sh
   git clone https://github.com/your-username/To-Do-App.git
   cd To-Do-App
   ```
2. **Database Setup:**
   - Ensure MySQL is running and create `todo_db`.
   - Update `application.properties` with credentials.
3. **Run the Application:**
   ```sh
   mvn spring-boot:run
   ```

## API Endpoints

| Method | Endpoint                   | Description          |
| ------ | -------------------------- | -------------------- |
| POST   | /api/todos                 | Add a new To-Do      |
| GET    | /api/todos/{id}            | Get a specific To-Do |
| GET    | /api/todos                 | Get all To-Dos       |
| PUT    | /api/todos/{id}            | Update a To-Do       |
| DELETE | /api/todos/{id}            | Delete a To-Do       |
| PATCH  | /api/todos/{id}/complete   | Mark as complete     |
| PATCH  | /api/todos/{id}/incomplete | Mark as incomplete   |

## Security

- JWT authentication is required.
- Admins can manage all To-Dos.

---

### Author

Your Name - [GitHub](https://github.com/your-username)

