# DP-800 Practice Question Bank

## Part 5 – Deployment & CI/CD (Questions 91–105)

> References are based on Microsoft Learn / Microsoft Docs topics covered by the DP-800 study guide.

---

## Question 91

What is the primary purpose of a SQL Database Project?

A. Store production data
B. Manage database schema as source code
C. Encrypt database objects
D. Monitor query performance

**Answer:** B. Manage database schema as source code

**Reference:** Microsoft Learn – SQL Database Projects

---

## Question 92

Which approach is promoted by SQL Database Projects?

A. Database-first only
B. Infrastructure-only deployments
C. Database schema as code
D. Manual production updates

**Answer:** C. Database schema as code

**Reference:** Microsoft Learn – SQL Database Projects

---

## Question 93

Why should database project files be stored in source control?

A. To improve query performance
B. To track changes, collaborate, and maintain history
C. To encrypt database objects
D. To replace backups

**Answer:** B. To track changes, collaborate, and maintain history

**Reference:** Microsoft Learn – Source Control Fundamentals

---

## Question 94

Which source control system is commonly used with Azure DevOps and GitHub?

A. LDAP
B. Git
C. Kerberos
D. OAuth

**Answer:** B. Git

**Reference:** Microsoft Learn – Git Fundamentals

---

## Question 95

What is the purpose of a branch in Git?

A. Encrypt source code
B. Allow isolated development without affecting the main codebase
C. Create backups automatically
D. Deploy directly to production

**Answer:** B. Allow isolated development without affecting the main codebase

**Reference:** Microsoft Learn – Git Branching

---

## Question 96

What is a pull request primarily used for?

A. Database backup restoration
B. Reviewing and validating proposed changes before merging
C. Rebuilding indexes
D. Encrypting secrets

**Answer:** B. Reviewing and validating proposed changes before merging

**Reference:** Microsoft Learn – Pull Requests

---

## Question 97

Which practice helps reduce deployment defects by requiring peer review?

A. Table Partitioning
B. Pull Requests
C. Query Store
D. Dynamic Data Masking

**Answer:** B. Pull Requests

**Reference:** Microsoft Learn – Pull Requests

---

## Question 98

What is schema drift?

A. Database encryption failure
B. Differences between expected schema and actual deployed schema
C. Index fragmentation
D. Query plan regression

**Answer:** B. Differences between expected schema and actual deployed schema

**Reference:** Microsoft Learn – Schema Drift

---

## Question 99

Why is schema drift problematic?

A. It improves performance unexpectedly
B. It can cause deployment inconsistencies and unexpected behavior
C. It removes indexes automatically
D. It disables authentication

**Answer:** B. It can cause deployment inconsistencies and unexpected behavior

**Reference:** Microsoft Learn – Schema Drift

---

## Question 100

What is the primary purpose of Continuous Integration (CI)?

A. Perform backups continuously
B. Automatically validate and build changes when code is committed
C. Encrypt application secrets
D. Manage user permissions

**Answer:** B. Automatically validate and build changes when code is committed

**Reference:** Microsoft Learn – CI/CD Fundamentals

---

## Question 101

What is the primary purpose of Continuous Deployment (CD)?

A. Deploy validated changes consistently to target environments
B. Create indexes automatically
C. Generate execution plans
D. Configure Row-Level Security

**Answer:** A. Deploy validated changes consistently to target environments

**Reference:** Microsoft Learn – CI/CD Fundamentals

---

## Question 102

What is a deployment pipeline?

A. A backup chain
B. An automated process that moves validated changes through environments
C. A security boundary
D. A database constraint

**Answer:** B. An automated process that moves validated changes through environments

**Reference:** Microsoft Learn – Azure DevOps Pipelines

---

## Question 103

Which practice is recommended for storing secrets such as connection strings and credentials?

A. Store them directly in source code
B. Save them in README files
C. Use a secure secrets management solution such as Azure Key Vault
D. Store them in SQL comments

**Answer:** C. Use a secure secrets management solution such as Azure Key Vault

**Reference:** Microsoft Learn – Azure Key Vault

---

## Question 104

Why should automated testing be included in a deployment pipeline?

A. To increase database size
B. To validate changes and reduce deployment risk
C. To create indexes automatically
D. To improve encryption strength

**Answer:** B. To validate changes and reduce deployment risk

**Reference:** Microsoft Learn – DevOps Testing Practices

---

## Question 105

A development team wants database changes to be versioned, peer-reviewed, automatically validated, and consistently deployed across environments. Which approach best meets these requirements?

A. Manual schema changes in production
B. Database DevOps using SQL Database Projects, Git, and CI/CD pipelines
C. Weekly backup verification only
D. Query Store monitoring

**Answer:** B. Database DevOps using SQL Database Projects, Git, and CI/CD pipelines

**Explanation:** The DP-800 study guide emphasizes modern database development practices using source control, automated validation, testing, and deployment pipelines.

**Reference:** Microsoft Learn – SQL Database Projects and DevOps Practices

---

## DP-800 CI/CD Cheat Sheet

### Core Concepts

| Concept              | Purpose              |
| -------------------- | -------------------- |
| SQL Database Project | Schema as Code       |
| Git                  | Version Control      |
| Branch               | Isolated Development |
| Pull Request         | Code Review          |
| CI                   | Build & Validate     |
| CD                   | Deploy Changes       |
| Pipeline             | Automation           |
| Azure Key Vault      | Secrets Management   |

---

### Common DP-800 Scenario Questions

**Need version-controlled database schema**
→ SQL Database Project

**Need peer review before merge**
→ Pull Request

**Need automated validation after commit**
→ Continuous Integration

**Need automated deployments**
→ Continuous Deployment

**Need secure storage for credentials**
→ Azure Key Vault

**Production differs from source repository**
→ Schema Drift

---

### Score Guide

* 14–15 Correct: Exam Ready
* 11–13 Correct: Strong Understanding
* 8–10 Correct: Review CI/CD Concepts
* Below 8: Revisit DevOps Objectives
