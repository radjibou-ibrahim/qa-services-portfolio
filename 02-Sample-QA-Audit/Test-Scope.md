# QA Audit Scope — OrangeHRM Demo

Application: OrangeHRM Demo
URL: https://opensource-demo.orangehrmlive.com/web/index.php/auth/login
Purpose: Independent manual QA demonstration project.

> This is a personal QA demonstration project. It is not affiliated with or commissioned by OrangeHRM.

## Objective
Evaluate selected authentication, navigation and employee-management workflows and document confirmed defects with reproducible evidence.

## In Scope
- Login: valid, invalid and empty credentials
- Logout
- Dashboard and main navigation
- PIM / Employee List
- Employee search
- Add Employee form
- Required-field validation
- Employee creation and retrieval
- Exploratory edge cases and basic UI/UX checks

## Out of Scope
- API testing
- SQL/database testing
- Performance/load testing
- Security penetration testing
- Mobile testing
- Full regression of every OrangeHRM module

## Approach
Functional, positive, negative, exploratory, usability/UI and edge-case testing.

## Environment

- **Application:** OrangeHRM Public Demo
- **Browser:** Google Chrome
- **Operating System:** Windows
- **Environment:** Public Demo

> Testing results are limited to the functionality, data and behavior available in the public demo environment at the time of testing.

---

## Evidence rule
Only reproducible, evidence-backed defects will be reported. No defects will be invented.

---

[← Back to QA Audit](./README.md)

[View Test Scenarios →](./Test-Scenarios.xlsx)
