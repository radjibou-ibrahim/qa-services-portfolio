# Test Process

## Overview

This document describes the standard process used to execute manual QA testing activities.

The process is designed to provide structured, traceable and evidence-based testing while remaining adaptable to the client's product, requirements, priorities and timeline.

---

# 1. Test Preparation

Before execution begins, the testing context is reviewed and confirmed.

### Activities

- Review the agreed scope
- Review available requirements
- Review acceptance criteria
- Confirm application access
- Confirm test credentials
- Confirm test environment
- Confirm required test data
- Review known issues
- Confirm testing objectives
- Confirm deliverables
- Confirm testing deadline

### Output

- Confirmed testing scope
- Confirmed environment
- Confirmed access and test data
- Testing preparation checklist

---

# 2. Requirements Review

Requirements are reviewed to determine what should be tested.

### Activities

- Identify functional requirements
- Identify business rules
- Identify expected behaviors
- Identify acceptance criteria
- Identify dependencies
- Identify potential risks
- Identify ambiguous or unclear requirements

When requirements are unclear, clarification should be requested before testing whenever possible.

---

# 3. Test Scope Definition

The features and workflows to be tested are explicitly defined.

### In Scope

Features and behaviors included in the agreed testing activities.

### Out of Scope

Features and activities that are not included in the agreed testing activities.

Clearly defining the scope helps prevent misunderstandings regarding the expected testing coverage.

---

# 4. Test Scenario Design

Test scenarios are created to represent the main conditions and workflows that need to be verified.

### Scenario Coverage

Depending on the project, scenarios may cover:

- Main business workflows
- Positive conditions
- Negative conditions
- Validation rules
- Boundary conditions
- Error handling
- Navigation
- User roles and permissions
- Exploratory areas
- Risk-based areas

### Output

- Test Scenarios

---

# 5. Test Case Design

Detailed test cases are created when the selected service requires structured test execution.

Each test case may contain:

- Test Case ID
- Requirement ID
- Scenario ID
- Test Case Title
- Preconditions
- Test Data
- Test Steps
- Expected Result
- Actual Result
- Status
- Evidence ID
- Bug ID
- Comments

Test cases should be clear, reproducible and independently executable whenever practical.

### Output

- Test Cases

---

# 6. Test Data Preparation

Test data is prepared according to the required test conditions.

### Test Data May Include

- Valid values
- Invalid values
- Empty values
- Boundary values
- Existing records
- Non-existing records
- Special characters
- Long input values
- User accounts
- Business-specific data

Test data must be appropriate for the environment and must not unnecessarily expose confidential information.

### Output

- Test Data

---

# 7. Test Environment Verification

Before execution, the environment is checked.

### Verification

- Application is accessible
- Required pages are available
- Test accounts work
- Required permissions are available
- Test data is accessible
- Browser/device is available
- Application version is confirmed when applicable

If a required dependency is unavailable, the affected test may be marked **BLOCKED**.

---

# 8. Test Execution

Test cases are executed using the defined test data and environment.

### Execution Steps

For each test case:

1. Review the preconditions.
2. Prepare the required test data.
3. Execute the test steps.
4. Observe the application behavior.
5. Compare the actual result with the expected result.
6. Record the actual result.
7. Assign the test status.
8. Record evidence when applicable.
9. Report a confirmed defect when necessary.

---

# 9. Test Status

Each executed test case receives an appropriate status.

### PASS

The observed behavior matches the expected result.

### FAIL

The observed behavior differs from the expected result and the deviation is confirmed as a defect.

### BLOCKED

The test cannot be completed because of an external dependency, access problem, environment issue or another blocking condition.

### NOT RUN

The test has not yet been executed.

---

# 10. Evidence Collection

Evidence is collected when it provides useful support for the test result or defect.

### Possible Evidence

- Screenshots
- Screen recordings
- Error messages
- Logs
- Relevant application information
- Execution records

### Evidence Rules

Evidence should:

- Be directly related to the test
- Be clear and understandable
- Support the reported result
- Avoid unnecessary sensitive information
- Use consistent naming
- Be traceable to the relevant test case

Only actual evidence is included.

Evidence must never be fabricated or modified in a way that misrepresents the observed behavior.

---

# 11. Defect Identification

When the actual result differs from the expected result, the issue is analyzed before reporting it.

### Verification

The tester checks:

- Is the expected behavior clearly defined?
- Is the behavior reproducible?
- Is the issue caused by the application?
- Is the issue already known?
- Is the issue caused by the test environment?
- Is additional information required?

Only sufficiently confirmed deviations should be reported as defects.

---

# 12. Defect Reporting

Confirmed defects are documented using the agreed defect management process.

### Typical Information

- Bug ID
- Summary
- Environment
- Preconditions
- Steps to Reproduce
- Expected Result
- Actual Result
- Severity
- Priority
- Evidence
- Related Requirement
- Related Test Case
- Status

The defect should contain enough information for another person to understand and reproduce the issue.

---

# 13. Exploratory Testing

Exploratory testing may be performed in addition to predefined test cases.

The tester explores the application using knowledge of the product, risks and potential user behavior.

### Exploratory Testing May Focus On

- Unexpected inputs
- Edge cases
- Navigation
- Error handling
- Usability issues
- Workflow inconsistencies
- Data handling
- Areas with higher perceived risk

Exploratory testing does not replace planned testing when structured coverage is required.

---

# 14. Retesting

Retesting is performed after a reported defect has been fixed.

### Process

1. Review the original defect.
2. Verify the updated application.
3. Repeat the original reproduction steps.
4. Confirm whether the expected behavior is now observed.
5. Record the result.
6. Update the defect status.

### Possible Results

- Fixed
- Reopened
- Cannot Reproduce
- Not Fixed
- Deferred

---

# 15. Regression Testing

Regression testing verifies that changes have not negatively affected previously working functionality.

### Regression Scope

Regression coverage depends on:

- Nature of the change
- Affected functionality
- Business risk
- Previous defects
- Project scope
- Available testing time

Regression testing may be targeted rather than a complete application regression.

---

# 16. Test Completion

Testing is completed when the agreed testing activities have been performed or when the defined exit conditions are reached.

### Completion Review

The tester reviews:

- Executed test cases
- PASS results
- FAIL results
- BLOCKED tests
- Defects
- Retesting results
- Regression results
- Evidence
- Remaining limitations
- Risks

---

# 17. Test Metrics

Depending on the project, test metrics may include:

- Total test cases
- Executed test cases
- Passed test cases
- Failed test cases
- Blocked test cases
- Not executed test cases
- Pass rate
- Number of confirmed defects
- Defects by severity
- Defects by priority
- Retesting results

Metrics should be presented together with their context and limitations.

---

# 18. QA Reporting

The testing results are summarized in the agreed QA deliverable.

### QA Report May Include

- Testing objective
- Scope
- Environment
- Testing approach
- Test coverage
- Execution results
- Defect summary
- Evidence references
- Retesting results
- Regression results
- Risks
- Limitations
- Recommendations
- QA conclusion

The report should clearly distinguish between confirmed defects, blocked tests, observations and limitations.

---

# 19. Client Handover

At the end of the testing activity, the agreed deliverables are provided to the client.

### Possible Deliverables

- Test Plan
- Test Scenarios
- Test Cases
- Test Data
- Test Execution Results
- Bug Reports
- Evidence
- Retesting Results
- Regression Results
- QA Test Summary
- QA Audit Report

Only the deliverables agreed upon before testing are included.

---

# Complete Test Process

The complete structured process can be represented as:

```text
Client & Product Understanding
            ↓
Requirements Review
            ↓
Scope Definition
            ↓
Test Scenario Design
            ↓
Test Case Design
            ↓
Test Data Preparation
            ↓
Environment Verification
            ↓
Test Execution
            ↓
Evidence Collection
            ↓
Defect Identification
            ↓
Defect Reporting
            ↓
Retesting
            ↓
Regression Testing
            ↓
Test Completion
            ↓
QA Reporting
            ↓
Client Handover
```
Not every project requires every stage.
The process is adapted according to the selected QA service, project scope, application type, requirements, risks, timeline and client expectations.

---

# Quality Principles
The testing process follows these principles:
- Requirements-driven testing
- Risk-based thinking
- Reproducible testing
- Evidence-based reporting
- Clear traceability
- Objective communication
- No fabricated defects or evidence
- Protection of confidential information
- Appropriate testing coverage
- Continuous improvement

  

