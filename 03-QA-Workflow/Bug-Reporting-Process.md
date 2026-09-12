# Bug Reporting Process

## Overview

This document describes the standard process used to identify, verify, document and communicate software defects.

The objective is to provide clear, reproducible and evidence-based bug reports that help developers understand and resolve identified issues efficiently.

A bug should only be reported when the observed behavior is sufficiently confirmed and differs from the expected behavior.

---

# 1. Identify the Issue

When unexpected behavior is observed, the tester first determines whether it may represent a defect.

### Initial Questions

- What happened?
- What was expected?
- Is the expected behavior defined?
- Can the issue be reproduced?
- Does the issue affect the application or the test environment?
- Is the issue already known?
- Is additional information required?

An unexpected behavior should not automatically be classified as a confirmed defect.

---

# 2. Reproduce the Issue

The issue should be reproduced before being reported whenever possible.

### Reproduction Process

1. Repeat the same actions.
2. Use the same test data.
3. Verify the same environment.
4. Confirm the same result.
5. Repeat the test when necessary.
6. Record the relevant observations.

### Reproducibility

The report should indicate whether the issue is:

- Always reproducible
- Frequently reproducible
- Intermittently reproducible
- Not reproducible

If the issue cannot be confirmed, it should not be presented as a confirmed defect without sufficient evidence.

---

# 3. Verify the Expected Result

The expected result must be based on an appropriate reference.

Possible references include:

- Requirements
- User stories
- Acceptance criteria
- Business rules
- Specifications
- Approved designs
- Documented application behavior

If no clear expected behavior exists, clarification may be required before reporting the issue.

---

# 4. Check for Existing Defects

Before creating a new bug report, check whether the issue has already been reported.

### Check

- Existing Jira issues
- GitHub Issues
- Client defect tracking system
- Known issues documentation

If an existing defect describes the same problem, the new observation should be linked to or added to the existing issue instead of creating an unnecessary duplicate.

---

# 5. Collect Evidence

Evidence should support the observed behavior.

### Possible Evidence

- Screenshot
- Screen recording
- Error message
- Log
- Relevant application information
- Test execution record

### Evidence Requirements

Evidence should be:

- Clear
- Relevant
- Authentic
- Traceable
- Related to the reported behavior

Sensitive client information must be removed or protected when necessary.

---

# 6. Create the Bug Report

A bug report should contain enough information for another person to understand and reproduce the issue.

### Standard Bug Report Structure

```text
Bug ID:
Summary:
Environment:
Preconditions:
Steps to Reproduce:
Expected Result:
Actual Result:
Severity:
Priority:
Evidence:
Requirement ID:
Test Case ID:
Reproducibility:
Status:
Additional Information:
```

--

## 7. Write a Clear Summary

The summary should describe the problem concisely.

### Recommended Structure

`[Area] + [Observed Problem] + [Relevant Condition]`

### Example

`[Checkout] Order confirmation message is not displayed after completing payment`

A good summary should allow the reader to understand the main problem without opening the complete report.

---

## 8. Write Reproducible Steps

Steps to reproduce should be:

- Numbered
- Clear
- Specific
- Sequential
- Easy to follow

### Example

1. Log in with a valid customer account.
2. Add a product to the cart.
3. Open the cart.
4. Proceed to checkout.
5. Enter valid checkout information.
6. Complete the order.

Avoid unnecessary actions that are not required to reproduce the issue.

---

## 9. Expected vs Actual Result

The distinction between expected and actual behavior must be explicit.

### Expected Result

Describe what the application should do.

### Actual Result

Describe what the application actually does.

### Example

**Expected Result**

The order confirmation page is displayed after the order is completed.

**Actual Result**

The order is completed, but the expected confirmation page is not displayed.

Do not mix the expected and actual results.

---

## 10. Severity

Severity describes the impact of the defect on the application or user.

A project may use its own severity classification.

### Typical Classification

#### Critical

The defect causes a critical failure and prevents essential application functionality.

**Examples may include:**

- Application unavailable
- Critical workflow completely unusable
- Severe data loss

#### High

The defect has a major functional or business impact.

**Examples may include:**

- Important workflow cannot be completed
- Major functionality is unusable
- Significant business operation is affected

#### Medium

The defect affects functionality but does not completely prevent the main workflow.

**Examples may include:**

- Incorrect validation
- Important UI behavior issue
- Partial functionality failure

#### Low

The defect has limited functional or user impact.

**Examples may include:**

- Minor UI issue
- Cosmetic problem
- Small usability inconsistency

Severity should be based on the actual impact rather than personal preference.

---

## 11. Priority

Priority indicates how urgently the defect should be addressed.

### Typical Classification

#### P1 — High Priority

The issue should be addressed as soon as possible.

#### P2 — Medium Priority

The issue should be addressed in the normal defect resolution cycle.

#### P3 — Low Priority

The issue can be addressed when resources are available.

Severity and priority are different concepts.

A defect may have high severity but lower priority depending on the business context.

---

## 12. Defect Status

The status depends on the client's workflow.

Typical statuses include:

```text
Open
↓
In Progress
↓
Fixed
↓
Ready for Retest
↓
Retested
↓
Closed
```
Other possible outcomes include:
- Reopened
- Cannot Reproduce
- Duplicate
- Deferred
- Rejected
- Won't Fix
The client's existing defect management workflow should be followed when one is available.

---

## 13. Retesting a Fixed Defect

After a defect is marked as fixed, the tester performs a retest.

### Retest Process

- Review the original bug report.
- Use the same environment when possible.
- Use the same test data.
- Repeat the reproduction steps.
- Verify the expected result.
- Record the result.
- Update the defect status.

### Result

If the issue is resolved:

```text
Fixed → Retested → Closed
```
If the issue still exists:

```text
Fixed → Retested → Reopened
```
---

## 14. Regression Verification
After a defect fix, relevant functionality may also be tested to ensure that the change did not introduce another problem.
Regression testing should focus on areas affected by:
- The defect fix
- Related functionality
- Shared components
- Connected workflows
- High-risk areas
The regression scope depends on the project and agreed testing objectives.

---

## 15. Traceability
Whenever applicable, defects should be linked to the relevant testing artifacts.

```text
Requirement
     ↓
Test Scenario
     ↓
Test Case
     ↓
Test Execution
     ↓
Bug Report
     ↓
Retesting
     ↓
Regression
```
Traceability makes it easier to understand the origin, impact and resolution of a defect.

---

## 16. Bug Reporting Rules

The following rules should always be followed:

- Report facts, not assumptions.
- Confirm the issue before reporting whenever possible.
- Clearly separate expected and actual results.
- Provide reproducible steps.
- Include relevant evidence.
- Use appropriate severity and priority.
- Avoid duplicate reports.
- Link the defect to the relevant test case when applicable.
- Protect confidential information.
- Do not fabricate evidence.
- Do not exaggerate the impact of an issue.
- Clearly document limitations that prevent confirmation.

---

## 17. When NOT to Report a Confirmed Bug

An issue should not be presented as a confirmed defect when:

- The expected behavior is unknown.
- The issue cannot be sufficiently reproduced.
- The behavior is caused by the test environment.
- The behavior is an already-known limitation.
- The available evidence is insufficient.
- The issue is based only on an assumption.

In these situations, the observation may instead be documented as:

- Test limitation
- Blocked test
- Observation
- Clarification request
- Known issue

---

## 18. Bug Report Quality Checklist

Before submitting a bug report, verify:

- [ ] The issue has been reproduced.
- [ ] Expected behavior is clearly defined.
- [ ] Actual behavior is clearly described.
- [ ] Steps to reproduce are complete.
- [ ] Environment is specified.
- [ ] Test data is identified when relevant.
- [ ] Evidence is attached when applicable.
- [ ] Severity is assigned.
- [ ] Priority is assigned when applicable.
- [ ] Requirement is linked when applicable.
- [ ] Test case is linked when applicable.
- [ ] Duplicate issues have been checked.
- [ ] Sensitive information has been protected.
- [ ] The report contains no unsupported assumptions.

---

## 19. Bug Report Lifecycle
The standard lifecycle can be represented as:

```text
Unexpected Behavior
        ↓
Initial Analysis
        ↓
Reproduction
        ↓
Expected Result Verification
        ↓
Existing Bug Check
        ↓
Evidence Collection
        ↓
Bug Report
        ↓
Developer Review / Fix
        ↓
Retesting
        ↓
Regression Verification
        ↓
Closed / Reopened
```
---

## 20. Final Principle

A good bug report is not simply a description of something that went wrong.

It should provide enough objective information for the team to:

- Understand the problem
- Reproduce the problem
- Assess its impact
- Prioritize the problem
- Fix the problem
- Verify the fix

The goal of bug reporting is to improve product quality through clear, factual and actionable information.

---

## 📬 Contact

**Radjibou IBRAHIM**  
Junior QA Manual Tester | Software Testing & Quality Assurance

**LinkedIn:**  
https://www.linkedin.com/in/radjibou-ibrahim

**GitHub:**  
https://github.com/radjibou-ibrahim

**Email:**  
ibrahimradjibou@gmail.com 
