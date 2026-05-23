# 2026 Comeback — API Testing Automation Portfolio

## 📌 Project Overview

This repository showcases my QA Automation and API Testing practice as part of my 2026 QA comeback roadmap.

## 🧭 Repository Structure

This repository contains two QA domains:

### 1. API Automation Framework (CI/CD Ready)
Located in:
Dockerized-API-QA/

Includes:
- Postman + Newman automation
- GitHub Actions CI pipeline
- Multi-environment testing (ReqRes, DummyJSON)
- Dockerized execution
- HTML reporting

---

### 2. Local API Testing & QA Practice Lab
Located in:
Local APIs/

Includes:
- Manual API testing cases
- Bug reports
- Local JSON server data
- Postman exploratory collections
- Test design documentation

It demonstrates a real-world API testing workflow using:

- Manual API testing (Postman)
- Automated API execution (Newman)
- CRUD lifecycle validation
- Negative & edge case testing
- Dockerized test execution
- Test design and documentation practices
- HTML reporting and execution analysis

A local JSON Server API is used to simulate a backend system for full CRUD testing.

---

## 🛠 Technologies & Tools

- Postman
- Newman (CLI automation runner)
- Docker & Docker Compose
- JSON Server (local API simulation)
- REST API Testing
- JavaScript (Postman test scripts)
- Git & GitHub
- Manual QA methodologies

---

## 🧪 Test Coverage

### 🔹 CRUD Operations
- Create user
- Retrieve user data
- Update user information
- Delete user
- End-to-end lifecycle validation

---

### 🔹 Authentication & Input Validation
- Valid login scenarios
- Invalid credentials
- Missing fields validation
- Empty input handling

---

### 🔹 Negative Testing
- Invalid request payloads
- Non-existent resource access
- Incorrect endpoints
- Error response validation

---

### 🔹 Boundary & Edge Cases
- Empty values
- Maximum/minimum input lengths
- Invalid formats
- Missing parameters

---

### 🔹 Security-Oriented Scenarios
- Basic SQL injection test scenarios
- Unauthorized access handling
- Input sanitization checks

---

## 📂 Project Structure

```txt
API Testing/
│
├── .github
│   ├── workflows
│
├── Dockerized-API-QA/
│   ├── api/
│
│   ├── newman/
│     ├── collections/
│       ├── dummyjson.json
│       ├── reqres.json
│
│     ├── environments/
│       ├── dummyjson.env.json
│       ├── reqres.env.json
│
│     ├── node_modules/
│
│     ├── reports/
│       ├── report.html
│
│     ├── package.json
│     ├── package-lock.json
│
│   ├── docker-compose.yml
│
├── Local APIs/
│   ├── bug-reports/
│     ├── api-bug-reports.md
│
│   ├── local-data/
│     ├── db.json
│
│   ├── newman/
│     ├── collection.json
│     ├── environment.json
│
│   ├── postman-local/
│     ├── reqres-api-tests-v1.postman_collection.json
│     ├── reqres-api-tests-v2-day2.postman_collection.json
│
│   ├── reports/
│     ├── newman-report.html
│
│   ├── test-cases/
│     ├── login-api-test-cases.md
│     ├── user-management-api-test-cases.md
│
│
│
├── screenshots/
│
│── readme.md

```
🚀 How to Run the Project
1️⃣ Start Local API
json-server db.json

API runs at:

http://localhost:3000
2️⃣ Run Postman Collection (Manual)

Import collection from:

postman/collections/
3️⃣ Run Automated Tests (Newman)
cd newman
newman run collection.json -e environment.json
4️⃣ Run Tests with Docker
docker compose up --build

This executes Newman inside a containerized environment.

5️⃣ Generate HTML Report
newman run collection.json -e environment.json -r htmlextra

Reports are saved in:

/reports
📊 Execution Summary
CRUD lifecycle fully automated
Dockerized Newman execution working
Collection runs inside containers
Negative scenarios covered
Stable PATCH update workflow
HTML reporting implemented
CI-ready structure prepared
🔄 Planned Improvements
Add GitHub Actions CI pipeline
Improve htmlextra reporting customization
Add multi-environment configuration
Expand negative test coverage
Add data-driven testing
Improve schema validation tests
Extend API scenarios beyond CRUD
🎯 Project Goals

This repository focuses on:

QA mindset and test design thinking
API validation and lifecycle testing
Automation with Newman
Dockerized QA workflows
Real-world QA workflow simulation
Professional documentation and portfolio readiness
📌 Notes
This project uses a local JSON Server for API simulation
Tests are designed to mimic real backend behavior
Newman is used for automated execution and reporting
Docker ensures reproducible test environments
