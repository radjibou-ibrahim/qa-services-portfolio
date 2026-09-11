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
Test Cases
     ↓
Test Data
     ↓
Test Execution
     ↓
Bug Identification
     ↓
Evidence Collection
     ↓
QA Audit Report
```
This structure demonstrates traceability between the testing objectives, test execution and reported findings.

---



