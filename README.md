# 2026 Comeback — API Testing Automation Portfolio

## 📌 Project Overview

This repository showcases my QA Automation and API Testing practice as part of my 2026 QA comeback roadmap.

The project focuses on building a real-world API testing workflow using:

- Manual API Testing (Postman)
- Automated API Execution (Newman)
- CRUD lifecycle validation
- Negative & edge case testing
- Test design and documentation practices
- Basic reporting and execution analysis

A local JSON Server API is used to simulate a real backend system for full CRUD testing.

---

## 🛠 Technologies & Tools

- Postman
- Newman (CLI automation runner)
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

### 🔹 Authentication & Input Validation
- Valid login scenarios
- Invalid credentials
- Missing fields validation
- Empty input handling

### 🔹 Negative Testing
- Invalid request payloads
- Non-existent resource access
- Incorrect endpoints
- Error response validation

### 🔹 Boundary & Edge Cases
- Empty values
- Maximum/minimum input lengths
- Invalid formats
- Missing parameters

### 🔹 Security-Oriented Scenarios
- SQL injection simulation
- Unauthorized access handling
- Input sanitization checks

---

## 📂 Project Structure

```text
API Testing/
│
├── postman/
│   ├── collections/
│   ├── environments/
│
├── newman/
│   ├── collection.json
│   ├── environment.json
│
├── reports/
│   ├── newman-report.html
│
├── test-cases/
│   ├── login-api-test-cases.md
│   ├── user-management-api-test-cases.md
│
├── bug-reports/
│   ├── api-bug-reports.md
│
├── screenshots/
│
├── local-api/
│   ├── db.json
🚀 How to Run the Project
1. Start Local API
json-server db.json

API runs at:

http://localhost:3000
2. Run Postman Collection (Manual)

Import collection from:

postman/collections/
3. Run Automated Tests (Newman)
cd newman
newman run collection.json -e environment.json
4. Generate HTML Report
newman run collection.json -e environment.json -r html

Reports are saved in:

/reports
📊 Execution Summary
✔ Total tests executed: 6+
✔ All core CRUD flows validated
✔ Negative scenarios covered
✔ Zero failures in current run
✔ Average execution time: ~400ms
🔄 Planned Improvements
Expand negative test coverage
Add data-driven testing (dynamic users)
Improve schema validation tests
Add CI/CD pipeline using GitHub Actions
Enhance reporting (multiple formats: HTML, JSON)
Extend API scenarios beyond CRUD
🎯 Project Goals

This repository focuses on improving:

QA mindset and test design thinking
API validation and lifecycle testing
Automation with Newman
Real-world QA workflow simulation
Professional documentation and portfolio readiness
📌 Notes
This project uses a local JSON Server for API simulation
Tests are designed to mimic real backend behavior
Newman is used as a lightweight CI-style execution tool