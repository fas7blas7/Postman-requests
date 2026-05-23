2026 Comeback — API Testing Automation Portfolio
📌 Project Overview

This repository showcases my QA Automation and API Testing practice as part of my 2026 QA comeback roadmap.
It demonstrates real-world API testing workflows using Postman, Newman, Docker, and manual QA practices.

🧭 Repository Structure

This repository contains two QA domains:

1. API Automation Framework (CI/CD Ready)

Located in:

Dockerized-API-QA/
Includes:
Postman + Newman automation
GitHub Actions CI pipeline (planned/in progress)
Multi-environment testing (ReqRes, DummyJSON)
Dockerized execution
HTML reporting (htmlextra)

▶ How to Run API Automation
Run without environment (local / collection variables)

From:

Dockerized-API-QA/newman/collections
npx newman run dummyjson.json -r cli,htmlextra

Run with environment (recommended / CI mode)

From project root:

npx newman run collections/dummyjson.json -e environments/dummyjson.env.json -r cli,htmlextra

2. Local API Testing & QA Practice Lab

Located in:

Local APIs/
Includes:
Manual API test cases
Bug reports
Local JSON Server setup
Postman exploratory collections
Test design documentation

A local JSON Server is used to simulate backend behavior for full CRUD testing.

🛠 Technologies & Tools
Postman
Newman (CLI automation runner)
Docker & Docker Compose
JSON Server (local API simulation)
REST API Testing
JavaScript (Postman test scripts)
Git & GitHub
Manual QA methodologies
🧪 Test Coverage
🔹 CRUD Operations
Create user
Retrieve user data
Update user information
Delete user
End-to-end lifecycle validation
🔹 Authentication & Input Validation
Valid login scenarios
Invalid credentials
Missing fields validation
Empty input handling
🔹 Negative Testing
Invalid request payloads
Non-existent resource access
Incorrect endpoints
Error response validation
🔹 Boundary & Edge Cases
Empty values
Max/min input lengths
Invalid formats
Missing parameters
🔹 Security-Oriented Scenarios
Basic injection test scenarios
Unauthorized access handling
Input sanitization checks
📂 Project Structure
API Testing/
│
├── Dockerized-API-QA/
│   ├── api/
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
│   ├── newman/
│   ├── postman-local/
│   ├── reports/
│   ├── test-cases/
│
├── screenshots/
│   ├── newman-cli-basic.png
│    ├── newman-cli-env.png
│    ├── report-basic.png
│    ├── report-env.png
│    ├── postman-collection.png

🚀 Additional Run Commands
Start Local API
json-server db.json
Run Postman Collection (manual)

Import collections from:

Local APIs/postman-local/
Run Dockerized Tests
docker compose up --build
Generate HTML Report
newman run collection.json -e environment.json -r htmlextra
📊 Execution Summary
CRUD lifecycle fully automated
Dockerized Newman execution working
Collection runs inside containers
Negative scenarios covered
PATCH update workflow stable
HTML reporting implemented
CI-ready structure prepared
🔄 Planned Improvements
GitHub Actions CI pipeline
Improved HTML reporting
Multi-environment expansion
More negative test coverage
Data-driven testing
Schema validation improvements
Extended API scenarios beyond CRUD
🎯 Project Goals
QA mindset & test design thinking
API lifecycle validation
Automation with Newman
Dockerized QA workflows
Real-world QA simulation
Professional portfolio readiness
📌 Notes
Uses local JSON Server for API simulation
Tests mimic real backend behavior
Newman used for automation execution
Docker ensures reproducibility

## 📌 Status
✔ Completed (core automation framework)  
🟡 CI/CD pipeline (next step)

## ⭐ Key Highlights

- Fully automated API test suite using Postman + Newman
- Environment-based execution (dev/staging simulation)
- HTML reporting with htmlextra
- CLI-based test execution for CI/CD readiness
- CRUD lifecycle validation
- Docker-ready execution structure

🔗 Repository

This project is available on GitHub:
https://github.com/fas7blas7/Postman-requests