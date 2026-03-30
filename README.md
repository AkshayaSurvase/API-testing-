# 🚀 API Testing using Postman & Newman

## 📌 Project Overview

This project demonstrates API testing using Postman and execution through Newman CLI.
A sample API endpoint is tested, and results are generated in both CLI and HTML report formats.

---

## 🛠️ Tools & Technologies Used

* Postman (API Testing Tool)
* Newman (CLI runner for Postman)
* Node.js
* HTML Reporter (newman-reporter-htmlextra)

---

## 📂 Project Files

* `project1.postman_collection.json` → Postman Collection
* `report.html` → Generated HTML Report

---

## ▶️ How to Run the Project

### 1. Install Dependencies

```bash
npm install -g newman
npm install -g newman-reporter-htmlextra
```

---

### 2. Run Collection using Newman

```bash
newman run project1.postman_collection.json -r cli,htmlextra
```

---

### 3. Generate HTML Report (Custom Path)

```bash
newman run project1.postman_collection.json -r cli,htmlextra --reporter-htmlextra-export report.html
```

---

## 📊 Test Scenario

* API Endpoint Tested:
  `https://restful-booker.herokuapp.com/booking`

* Test Performed:

  * Status Code Validation (200 OK)
  * Response Verification

---

## 📄 Report

The HTML report contains:

* Request details
* Response data
* Test results (Pass/Fail)
* Execution time

🎯 Key Learnings
1) API testing using Postman
2) Running collections via CLI (Newman)
3) Generating professional HTML reports
4) Handling errors and debugging
