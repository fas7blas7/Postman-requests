# 🚀 2026 QA Comeback - Postman API Collection

> A simple REST API testing collection created with Postman as part of my 2026 QA comeback journey.

---

# 📌 Project Overview

This collection demonstrates basic API testing operations against a local Task Board application using:

- ✅ GET Requests
- ✅ POST Requests
- ✅ PATCH Requests
- ✅ DELETE Requests

The project focuses on practicing:
- 🌐 REST API testing
- 🧪 CRUD operations
- 📬 Postman collections
- 🔍 Request validation
- ⚡ QA workflow fundamentals

---

# 🛠️ Technologies Used

| Tool | Purpose |
|------|----------|
| 📬 Postman | API Testing |
| 🌐 REST API | Backend communication |
| 🧾 JSON | Request body formatting |
| 💻 Localhost Server | Local API testing |
| 🔧 HTTP Methods | CRUD operations |

---

# 📂 Collection Endpoints

## 📥 GET - Retrieve All Tasks

```http
GET http://localhost:8080/api/tasks
```

✔️ Retrieves all available tasks from the task board.

---

## ➕ POST - Create a New Task

```http
POST http://localhost:8080/api/tasks/
```

### 📦 Request Body

```json
{
  "title": "Creating a task trough postman 2026 comeback",
  "description": "Testing API - post functionality"
}
```

✔️ Creates a new task inside the application.

---

## ✏️ PATCH - Edit Existing Task

```http
PATCH http://localhost:8080/api/tasks/7
```

### 📦 Request Body

```json
{
  "id": 7,
  "title": "Edited task",
  "description": "Testing API - PATCH functionality"
}
```

✔️ Updates an existing task by ID.

---

## ❌ DELETE - Remove Task

```http
DELETE http://localhost:8080/api/tasks/9
```

✔️ Deletes a task from the task board.

---

# 🎯 Learning Goals

This project helped reinforce knowledge in:

- ✅ API Testing
- ✅ CRUD Operations
- ✅ HTTP Methods
- ✅ JSON Payloads
- ✅ Postman Collections
- ✅ Backend Communication
- ✅ QA Testing Practices

---

# 📸 Example Workflow

```text
npm installation of environment
---
GET ➜ Create Task ➜ Edit Task ➜ Delete Task
```

---

# 📚 Future Improvements

- 🔐 Authentication testing
- 🧪 Automated API assertions
- ⚡ Newman CLI integration
- 🔄 CI/CD integration
- 📊 Test reporting
- 🐳 Dockerized API environment

---

# 👨‍💻 Author

QA Comeback Journey - 2026 🚀

Focused on:
- Manual QA
- API Testing
- Automation Fundamentals
- Continuous Improvement

---

# ⭐ Repository Purpose

This repository is part of my personal effort to refresh and strengthen my QA and API testing skills while building a cleaner and more professional GitHub portfolio.
