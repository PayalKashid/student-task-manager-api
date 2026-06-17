# Understanding Document

## Project Overview

I developed a Student Task Manager REST API using FastAPI. The application allows users to create, retrieve, update, and delete student-related tasks.

## Technologies Used

- FastAPI
- Python
- SQLAlchemy
- SQLite
- Pydantic
- Uvicorn

## Project Structure

### main.py
Contains all API routes.

### schemas.py
Defines request and response models using Pydantic.

### models.py
Defines database tables using SQLAlchemy.

### crud.py
Contains database operations.

### database.py
Configures the SQLite database connection.

## CRUD Operations

POST /tasks
Creates a task.

GET /tasks
Retrieves all tasks.

GET /tasks/{task_id}
Retrieves a specific task.

PUT /tasks/{task_id}
Updates a task.

DELETE /tasks/{task_id}
Deletes a task.

## Validation

Pydantic validation ensures that task titles contain between 3 and 100 characters. Invalid requests return a 422 error.

## Database

SQLite stores tasks in tasks.db. Data persists even after restarting the server.

## Challenges

Initially, understanding FastAPI project structure and environment setup was challenging. Through experimentation and debugging, I learned how the components work together.

## What I Learned

- Building REST APIs using FastAPI
- Request validation using Pydantic
- Database operations using SQLAlchemy
- Organizing backend projects
- Testing APIs using Swagger UI

## Conclusion

This project helped me understand the fundamentals of backend development and REST API design.