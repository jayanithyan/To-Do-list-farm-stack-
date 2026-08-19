# 🚀 FARM Stack Todo Application

A full-stack Todo application built using the **FARM Stack** — **FastAPI, React, and MongoDB** — with **Docker** and **Nginx** for containerization and reverse proxy configuration.

This project was built to gain practical experience in developing and connecting a modern **Python backend**, **React frontend**, and **NoSQL database** into a complete full-stack application.

---

## 📌 Project Overview

This application allows users to manage their tasks through a simple and responsive web interface.

The project demonstrates how a React frontend communicates with a FastAPI REST API, while MongoDB handles persistent data storage.

The entire application can be containerized and run using Docker Compose.

### ✨ Core Architecture

```text
                    ┌──────────────────┐
                    │      Client      │
                    │   React Frontend │
                    └────────┬─────────┘
                             │
                             ▼
                    ┌──────────────────┐
                    │      Nginx       │
                    │  Reverse Proxy   │
                    └────────┬─────────┘
                             │
                             ▼
                    ┌──────────────────┐
                    │     FastAPI      │
                    │     Backend      │
                    └────────┬─────────┘
                             │
                             ▼
                    ┌──────────────────┐
                    │     MongoDB      │
                    │     Database     │
                    └──────────────────┘
```

---

## 🛠️ Tech Stack

### Frontend

* React.js
* JavaScript
* HTML5
* CSS3

### Backend

* Python
* FastAPI
* REST API
* Uvicorn

### Database

* MongoDB

### DevOps & Infrastructure

* Docker
* Docker Compose
* Nginx

---

## ✨ Features

* ✅ Create new tasks
* ✅ View existing tasks
* ✅ Update task status
* ✅ Delete tasks
* ✅ Persistent MongoDB storage
* ✅ RESTful API architecture
* ✅ React-based frontend
* ✅ FastAPI backend
* ✅ Dockerized application
* ✅ Docker Compose orchestration
* ✅ Nginx reverse proxy
* ✅ Frontend-backend integration

---

## 📂 Project Structure

```text
FARM-Stack-Todo/
│
├── backend/
│   ├── main.py
│   ├── requirements.txt
│   └── ...
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── ...
│
├── nginx/
│   └── nginx.conf
│
├── docker-compose.yml
├── Dockerfile
├── .gitignore
└── README.md
```


---

## 🔄 How It Works

### 1. User Interaction

The user interacts with the Todo application through the React frontend.

### 2. API Request

React sends HTTP requests to the FastAPI backend.

For example:

```text
POST /todos
GET /todos
PUT /todos/{id}
DELETE /todos/{id}
```

### 3. FastAPI Processing

FastAPI receives the request, processes the data, and communicates with MongoDB.

### 4. MongoDB

MongoDB stores the Todo documents and provides persistent data storage.

### 5. Response

The backend sends the result back to React, which updates the UI.

---

## 🐳 Running the Project with Docker

### Prerequisites

Make sure you have installed:

* Docker
* Docker Compose
* Git

### Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

```bash
cd YOUR_REPOSITORY
```

### Start the Application

```bash
docker compose up --build
```

After the containers are running, open the application in your browser.

```text
http://localhost
```

### Stop the Application

```bash
docker compose down
```

---

## 🔌 API Endpoints

| Method   | Endpoint      | Description        |
| -------- | ------------- | ------------------ |
| `GET`    | `/todos`      | Retrieve all todos |
| `POST`   | `/todos`      | Create a new todo  |
| `PUT`    | `/todos/{id}` | Update a todo      |
| `DELETE` | `/todos/{id}` | Delete a todo      |

> Update these endpoints if your implementation uses different routes.

---

## 🧠 What I Learned

Building this project helped me understand how different parts of a full-stack application work together.

### Backend

* Building REST APIs using FastAPI
* Request/response handling
* API routing
* Connecting Python applications to MongoDB
* CRUD operations
* Running applications using Uvicorn

### Frontend

* React component architecture
* State management
* Calling REST APIs from React
* Handling asynchronous requests
* Connecting frontend applications with backend services

### Database

* MongoDB fundamentals
* Document-based data modeling
* CRUD operations
* Connecting MongoDB with a backend application

### DevOps

* Creating Docker containers
* Writing Dockerfiles
* Using Docker Compose
* Container-to-container communication
* Configuring Nginx as a reverse proxy

---

## 🎯 Project Goals

The main goals of this project were to:

* Understand full-stack application architecture
* Learn FastAPI development
* Practice React frontend development
* Work with MongoDB
* Understand REST API communication
* Learn Docker-based development
* Understand reverse proxy configuration using Nginx
* Deploy multiple application components as containers

---

## 🚀 Future Improvements

Possible improvements for future versions include:

* 🔐 User authentication and authorization
* 👤 User-specific Todo lists
* 🔎 Search and filtering
* 📊 Task analytics
* 🏷️ Task categories and priorities
* 📅 Due dates and reminders
* 🌙 Dark mode
* 🧪 Automated backend and frontend tests
* ⚡ Redis caching
* ☁️ Cloud deployment
* 🔄 CI/CD using GitHub Actions

---
g
```


## ⭐ If You Found This Project Useful

If this project helped you understand the FARM stack, consider giving the repository a ⭐.

---

## 📄 License

This project is intended for educational and learning purposes.
