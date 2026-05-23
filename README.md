# 2026 Comeback — API Testing Automation Portfolio

---

## 📌 Overview

This project demonstrates a **real-world API testing automation framework** built as part of my QA comeback roadmap.

It focuses on end-to-end API validation using automation, CI execution, and structured test design principles.

Built with:

Postman
Newman
Docker
GitHub Actions
JSON Server

---

## 🧭 Project Structure

```
API Testing/
│
├── Dockerized-API-QA/
│   ├── newman/
│   │   ├── collections/
│   │   ├── environments/
│   │   ├── reports/
│   │   ├── package.json
│   │   ├── docker-compose.yml
│
├── Local APIs/
│   ├── bug-reports/
│   ├── local-data/
│   ├── postman-local/
│   ├── test-cases/
│   ├── reports/
│
├── screenshots/
│   ├── newman-cli-basic.png
│   ├── newman-cli-env.png
│   ├── report-basic.png
│   ├── report-env.png
│   ├── postman-collection.png
```

---

## 🚀 CI/CD Pipeline

This project uses entity["software","GitHub Actions","CI/CD automation platform"] for continuous testing.

On every push to `main`:

1. Repository is checked out
2. Node.js environment is set up
3. Dependencies are installed
4. API tests are executed using entity["software","Newman","Postman CLI collection runner"]
5. HTML report is generated (htmlextra)
6. Report is uploaded as artifact

👉 CI Status is visible via badge at the top of this README

---

## 🧪 Test Coverage

### ✔ CRUD Operations

* Create user
* Read user data
* Update user information
* Delete user
* Full lifecycle validation

### ✔ Negative Testing

* Invalid endpoints
* Missing fields
* Non-existent resources
* Error response validation

### ✔ Boundary Testing

* Empty values
* Invalid formats
* Edge-case payloads

---

## ▶ How to Run

### Local Execution

```bash
cd Dockerized-API-QA/newman
newman run collections/dummyjson.json -r htmlextra
```

---

### With Environment

```bash
newman run collections/dummyjson.json \
-e environments/dummyjson.env.json \
-r htmlextra
```

---

### Docker Execution

```bash
docker compose up --build
```

---

## 📊 CI Execution Result

* Automated execution via entity["software","GitHub Actions","CI/CD automation platform"]
* HTML reports generated using Newman htmlextra reporter
* Artifacts stored per run

👉 View runs: [https://github.com/fas7blas7/Postman-requests/actions](https://github.com/fas7blas7/Postman-requests/actions)

---

## 📸 Execution Evidence

### CLI Execution

* Newman terminal output (local + CI)

### HTML Report

* htmlextra report dashboard
* request/response validation details

### Postman Collection

* Structured API test suite
* Environment variable usage

---

## ⭐ Key Highlights

* Fully automated API testing framework
* CI/CD integration with GitHub Actions
* Environment-based execution support
* Dockerized test execution
* HTML reporting (htmlextra)
* CRUD lifecycle validation
* Portfolio-ready QA structure

---

## 🛠 Technologies

entity["software","Postman","API testing and collaboration platform"] • entity["software","Newman","Postman CLI collection runner"] • entity["software","Docker","containerization platform"] • entity["software","GitHub Actions","CI/CD automation platform"] • entity["software","JSON Server","mock REST API server"] • REST API Testing • JavaScript • Git

---

## 📌 Status

✔ Completed (API automation framework) 🟢 CI/CD pipeline active

---

## 🔗 Repository

[https://github.com/fas7blas7/Postman-requests](https://github.com/fas7blas7/Postman-requests)