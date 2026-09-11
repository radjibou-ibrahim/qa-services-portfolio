# Sample QA Audit — OrangeHRM Demo

> Independent manual QA demonstration project focused on functional, exploratory and usability testing.

---

## 📌 Project Overview

This project demonstrates how I approach a real-world manual QA audit on a web application.

The application tested is the **OrangeHRM Demo**, a publicly available Human Resource Management System used here strictly for QA learning and portfolio demonstration purposes.

The audit focuses on selected authentication, navigation and employee-management workflows.

The objective is not to test the entire application, but to demonstrate a structured and practical QA process within a clearly defined scope.

---

## 🎯 Audit Objective

The main objectives of this audit are to:

- Validate selected critical user workflows
- Identify functional defects
- Verify positive and negative scenarios
- Explore potential edge cases
- Check basic UI/UX behavior
- Document reproducible defects
- Provide clear testing evidence
- Demonstrate a complete manual QA workflow

Only confirmed and reproducible defects supported by appropriate evidence are reported.

---

## 🌐 Application Under Test

**Application:** OrangeHRM Demo

**URL:**  
https://opensource-demo.orangehrmlive.com/web/index.php/auth/login

**Application Type:** Web Application

**Testing Type:** Independent Manual QA Audit

---

## 📋 Scope

### In Scope

The audit covers selected areas including:

- Login with valid credentials
- Login with invalid credentials
- Login with empty credentials
- Logout
- Dashboard
- Main navigation
- PIM / Employee List
- Employee search
- Add Employee form
- Required-field validation
- Employee creation
- Employee retrieval
- Exploratory edge cases
- Basic UI/UX checks

### Out of Scope

The following areas are excluded from this audit:

- API testing
- SQL/database testing
- Performance testing
- Load testing
- Security penetration testing
- Mobile testing
- Full regression testing of every OrangeHRM module

The complete scope is documented in:

`Test-Scope.md`

---

## 🧪 Testing Approach

The audit combines structured testing and exploratory investigation.

The following approaches are used where relevant:

- Functional testing
- Positive testing
- Negative testing
- Exploratory testing
- Usability testing
- UI checks
- Edge-case testing
- Basic boundary testing

The testing approach is adapted to the selected functionality and the defined audit scope.

---

## 🖥️ Test Environment

| Item | Environment |
|---|---|
| Application | OrangeHRM Demo |
| Browser | Google Chrome |
| Operating System | Windows |
| Testing Type | Manual |
| Environment | Public Demo |

---

## 🔄 QA Process

The audit follows a structured workflow:

```text
Test Scope
     ↓
Test Scenarios
     ↓
Test Execution
     ↓
Bug-Reports
     ↓
Evidence Collection
     ↓
QA Audit Report
```
This structure demonstrates traceability between the testing objectives, test execution and reported findings.

---

## 📊 Test Execution

Test execution results are recorded in:

`Test-Execution.xlsx`

Each executed test case is evaluated according to its actual result.

Possible statuses include:

- **PASS**
- **FAIL**
- **BLOCKED**
- **NOT RUN**

The final execution metrics are based on the actual recorded test results.

---

## 🐞 Defect Reporting

Confirmed defects are documented in:

`04-Bug-Reports/`

Each defect report may contain:

- **Bug ID**
- **Title**
- **Environment**
- **Preconditions**
- **Steps to Reproduce**
- **Expected Result**
- **Actual Result**
- **Severity**
- **Priority**
- **Evidence**
- **Status**

Only reproducible and evidence-backed defects are reported.

---

## 📸 Testing Evidence

Testing evidence is stored in:

`05-Evidence/`

Evidence may include:

- Screenshots
- Error messages
- Relevant UI states
- Other reproduction evidence

Evidence is linked to the relevant findings whenever applicable.

---

## 📦 Project Deliverables

This audit contains the following QA deliverables:

- `Test-Scope.md`
- `Test-Scenarios.xlsx`
- `Test-Execution.xlsx`
- `04-Bug-Reports/`
- `05-Evidence/`
- `QA-Audit-Report.pdf`

The documents demonstrate the different stages of a structured manual QA engagement.

---

## 🔗 Traceability

The project is organized to maintain traceability between the different QA activities:

```text
Test Scope
     ↓
Test Scenario
     ↓
Test Case
     ↓
Test Execution
     ↓
Bug-Reports
     ↓
Evidence
     ↓
QA Audit Report
```
This makes it possible to understand how identified defects relate to the tested functionality.

---

## 📈 Final QA Report
The final results of the audit are summarized in:
- QA-Audit-Report.pdf
- The report provides an overview of:
- Testing scope
- Testing approach
- Test environment
- Executed tests
- Test results
- Identified defects
- Severity and priority
- Evidence
- Key findings
- Testing limitations
- Final QA assessment
- The report reflects the actual results recorded during the audit.

---

## 🛠️ Tools
Tools used in this project include:
Google Chrome — Web application testing
Microsoft Excel — Test scenarios, test cases, test data and execution
GitHub — Project documentation and version control

---

## ⚠️ Testing Limitations
This project represents a limited QA audit and does not constitute a complete quality assessment of the OrangeHRM platform.
The conclusions apply only to:
- The tested functionality
- The defined scope
- The selected environment
- The available test data
- The testing period
- Untested functionality is outside the conclusions of this audit.

---
  
## 🔐 Disclaimer
This is an independent personal QA demonstration project.
It is not affiliated with, sponsored by, commissioned by, or endorsed by OrangeHRM.
The OrangeHRM Demo application is used solely for testing practice and portfolio demonstration.
No confidential or private client information is used in this project.

---

## 📁 Project Structure

02-Sample-QA-Audit/
│
├── README.md
├── Test-Scope.md
│
├── Test-Scenarios.xlsx
├── Test-Execution.xlsx
│
├── 04-Bug-Reports/
│
├── 05-Evidence/
│   ├── README.md
│   └── screenshots/
│
└── QA-Audit-Report.pdf

---

## 👤 Tester

**Radjibou IBRAHIM**  
Junior QA Manual Tester

### QA Focus

- Manual Testing
- Functional Testing
- Exploratory Testing
- Test Design
- Bug Reporting
- Regression Testing
- Web Application Testing

---

## 📞 Contact

📧 ibrahimradjibou@gmail.com  
📧 radjguerigui07@gmail.com

💼 **LinkedIn:**  
https://www.linkedin.com/in/radjibou-ibrahim

💻 **GitHub:**  
https://github.com/radjibou-ibrahim

---

## ⭐ Purpose of This Project

This project demonstrates my ability to organize and execute a structured manual QA audit, from defining the testing scope to documenting findings and delivering a final QA summary.

The focus is on clear testing, reproducible defects, traceability and useful QA reporting.
  
