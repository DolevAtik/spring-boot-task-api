# Spring Boot Task API

A simple RESTful API for managing tasks (Todo list), built with Spring Boot, Spring Data JPA, and H2 database.

## 🚀 Features
- Create, Read, Update, Delete (CRUD) tasks
- RESTful endpoints using Spring Web
- In-memory H2 database (no setup needed)
- JPA & Hibernate integration

## 📦 Tech Stack
- Java 17+
- Spring Boot 3.3.x
- Spring Web
- Spring Data JPA
- H2 Database

## 🛠️ Endpoints

### Get all tasks
```http
GET /tasks
```

### Get task by ID
```http
GET /tasks/{id}
```

### Create a task
```http
POST /tasks
Content-Type: application/json

{
  "title": "Finish project",
  "description": "Build REST API",
  "completed": false
}
```

### Update a task
```http
PUT /tasks/{id}
Content-Type: application/json

{
  "title": "Updated title",
  "description": "New description",
  "completed": true
}
```

### Delete a task
```http
DELETE /tasks/{id}
```

## ▶️ Getting Started

### Clone the repo
```bash
git clone https://github.com/DolevAtik/spring-boot-task-api.git
cd spring-boot-task-api
```

### Run the app
You can run the app from your IDE (IntelliJ recommended) or with Maven:
```bash
./mvnw spring-boot:run
```

### Access the API
```
http://localhost:8080/tasks
```

## 🧠 Notes
- Uses in-memory database (H2) — data resets on restart
- You can view the H2 console at:
```
http://localhost:8080/h2-console
```
Use `jdbc:h2:mem:testdb` as the JDBC URL

## 📄 License
This project is open-source and free to use.
