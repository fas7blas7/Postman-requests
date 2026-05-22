2026 Comeback — API Testing Automation Portfolio
📌 Project Overview

This repository showcases my QA Automation and API Testing practice as part of my 2026 QA comeback roadmap.

The project focuses on building a real-world API testing workflow using:

Manual API Testing (Postman)
Automated API Execution (Newman)
CRUD lifecycle validation
Negative & edge case testing
Dockerized test execution
Test design and documentation practices
HTML reporting and execution analysis

A local JSON Server API is used to simulate a real backend system for full CRUD testing.

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
Maximum/minimum input lengths
Invalid formats
Missing parameters
🔹 Security-Oriented Scenarios
Basic SQL injection test scenarios
Unauthorized access handling
Input sanitization checks

📂 Project Structure
API Testing/
│
├── docker/
│   ├── docker-compose.yml
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

This executes the Newman collection inside a containerized environment.

5️⃣ Generate HTML Report
newman run collection.json -e environment.json -r htmlextra

Reports are saved in:
/ reports

📊 Execution Summary

✔ CRUD lifecycle fully automated
✔ Dockerized Newman execution working
✔ Collection successfully runs inside containers
✔ Negative scenarios covered
✔ Current stable setup uses PATCH update requests
✔ HTML reporting prepared for future improvements
✔ Zero failures in latest successful execution

🔄 Planned Improvements
Add GitHub Actions CI pipeline
Improve htmlextra reporting customization
Add multi-environment configuration
Expand negative test coverage
Add data-driven testing
Improve schema validation tests
Extend API scenarios beyond CRUD

🎯 Project Goals

This repository focuses on improving:

QA mindset and test design thinking
API validation and lifecycle testing
Automation with Newman
Dockerized QA workflows
Real-world QA workflow simulation
Professional documentation and portfolio readiness

📌 Notes
This project uses a local JSON Server for API simulation
Tests are designed to mimic real backend behavior
Newman is used for automated API collection execution and reporting
Docker is used to ensure isolated and reproducible test execution environments
