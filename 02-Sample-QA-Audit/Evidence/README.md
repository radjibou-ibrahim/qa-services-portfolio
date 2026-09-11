# Test Evidence

This directory contains the evidence associated with the OrangeHRM Demo QA Audit.

## Evidence Convention

Each executed test case is associated with a unique Evidence ID.

```text
TC-001 → EVD-001
TC-002 → EVD-002
TC-003 → EVD-003
...
TC-024 → EVD-024
```
The Evidence IDs used in this directory are the same identifiers referenced in Test-Execution.xlsx.

---

## 📸 Evidence IDs

| Test Case | Evidence ID |
|---|---|
| TC-001 | EVD-001 |
| TC-002 | EVD-002 |
| TC-003 | EVD-003 |
| TC-004 | EVD-004 |
| TC-005 | EVD-005 |
| TC-006 | EVD-006 |
| TC-007 | EVD-007 |
| TC-008 | EVD-008 |
| TC-009 | EVD-009 |
| TC-010 | EVD-010 |
| TC-011 | EVD-011 |
| TC-012 | EVD-012 |
| TC-013 | EVD-013 |
| TC-014 | EVD-014 |
| TC-015 | EVD-015 |
| TC-016 | EVD-016 |
| TC-017 | EVD-017 |
| TC-018 | EVD-018 |
| TC-019 | EVD-019 |
| TC-020 | EVD-020 |
| TC-021 | EVD-021 |
| TC-022 | EVD-022 |
| TC-023 | EVD-023 |
| TC-024 | EVD-024 |

---

## 📸 Evidence and Test Execution

The Evidence IDs documented here correspond directly to the Evidence ID values recorded in the test execution file.

This allows each execution record to be traced to its corresponding evidence reference.

```text
Test Case
    ↓
Evidence ID
    ↓
Test Execution
```

---

## 🚫 Evidence for Blocked Test Case

**TC-018**

**Test Case:** TC-018  
**Evidence ID:** EVD-018  
**Status:** BLOCKED

The result could not be confirmed as a functional defect because the public demo environment may not guarantee data persistence between sessions.

The test should be repeated immediately after TC-017 within the same active session, or executed in a persistent test environment.

Therefore:

- EVD-018 remains a valid evidence reference.
- TC-018 remains BLOCKED.
- No defect is reported based solely on this result.
  
---

## 📸 Screenshot Naming Convention

If screenshots are added to this directory, they should use the corresponding Evidence ID as the filename:

```text
EVD-001.png
EVD-002.png
EVD-003.png
...
EVD-024.png
```
This makes the evidence easy to identify and trace back to the relevant test case. 

---

## 📋 Evidence Policy
Only evidence actually collected during the testing activity should be referenced.
No screenshots, videos or other evidence should be fabricated or created solely to complete the documentation.
Where evidence is unavailable, the corresponding test execution record remains the source of truth.

---

## 📊 Current Evidence Status

The Evidence IDs EVD-001 through EVD-024 are defined and referenced in the test execution documentation.
The screenshot files are not currently included in this repository.
If the original screenshots become available, they can be added to:
Evidence/screenshots/
using the established Evidence ID naming convention.
