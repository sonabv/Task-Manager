# Task-Manager
This is a backend service that mimics Unix-like process management via RESTful API's using java, Spring Boot and sql*Plus. Inspired by command like 'ls', 'fork', and 'kill', the service allows clients to create, list, fetch, update, and delete lightweight "tasks".

# Feaures
- GET/tasks -> List all tasks(like 'ls')
- POST/tasks -> Create a new task(like 'fork')
- GET/tasks/{id} -> Get details of a single task
- PATCH/tasks/{id}/status -> Update the task's status
- DELETE/tasks/{id} -> Delete a task(like 'kill')

   # Tech Stack
  - Java
  - Spring Boot
  - Oracle Database
  - JPA+ Spring Data
 
  # Table Structure

  CREATE TABLE TASKS(
  id VARCHAR2(36) PRIMARY KET,
  name VARCHAR2(100) NOT NULL,
  status VARCHAR2(20) DEFAULT 'running' NOT NULL,
  create_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
  );
