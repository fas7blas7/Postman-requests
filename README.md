# 🧪 QA API Testing Project (Postman) — 2026 Comeback

## 📌 Overview

This project is part of my QA comeback journey focused on Manual QA and API testing skills.
It demonstrates API testing using Postman, including positive and negative test scenarios, assertions, and response validation.

The goal is to simulate real QA work by validating REST API behavior, detecting inconsistencies, and ensuring response correctness.

---

## 🌐 API Used

This project uses the ReqRes mock API:

https://reqres.in/

ReqRes provides simulated REST endpoints for:

* User management
* Authentication
* CRUD operations
* Negative test scenarios

---

## 🧪 Tools Used

* Postman
* JavaScript (Postman Test Scripts)
* REST API
* ReqRes API (Mock backend)

---

## 📁 Project Structure

QA-API-Testing-Project/
│
├── postman-collection/
│ └── reqres-day2.postman_collection.json
│
├── test-cases/
│ └── (future manual test cases)
│
├── bug-reports/
│ └── (future bug reports)
│
└── README.md

---

## 📌 API Endpoints Tested

### 🟢 Users

* GET /api/users?page=2
* GET /api/users/{id}

### 🔐 Authentication

* POST /api/login

### 🔴 Negative Tests

* Missing password login
* Invalid credentials handling

---

## 🧪 Test Coverage

The following validations are included:

### ✔ Status Code Validation

* Ensuring correct HTTP responses (200, 400, etc.)

### ✔ Response Body Validation

* Checking presence of data fields
* Validating error messages
* Ensuring correct data structure

### ✔ Data Integrity Checks

* Array length validation
* Field format validation (e.g., avatar URL)

### ✔ Negative Testing

* Missing required fields
* Invalid login attempts

---

## 🧠 Example Test Snippet

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Response contains data array", function () {
    let jsonData = pm.response.json();
    pm.expect(jsonData.data).to.be.an("array");
});
```

---

## 🐞 Notes on API Behavior

During testing, some inconsistencies were observed in error handling responses.
Since ReqRes is a mock API, some responses may not reflect real backend validation logic.

These scenarios were still useful for practicing:

* negative testing
* response validation
* QA observation skills

---

## 🎯 Learning Objectives

This project helped me practice:

* REST API testing with Postman
* Writing automated test scripts
* Negative test scenario design
* API response validation
* QA thinking and bug identification mindset

---

## 🚀 Future Improvements

* Add Postman environment variables
* Add Newman CLI execution
* Integrate into CI pipeline (GitHub Actions)
* Add structured bug reports
* Expand test coverage with more edge cases

---

## 👨‍💻 Author

QA Engineer in training — 2026 Comeback Project
