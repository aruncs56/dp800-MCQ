# DP-800 Practice Question Bank

## Part 3 – Security (Questions 51–70)

> References are based on Microsoft Learn / Microsoft Docs topics covered in the DP-800 study guide.

---

## Question 51

What is the primary purpose of authentication in SQL Server and Azure SQL?

A. Determine what actions a user can perform
B. Verify the identity of a user or application
C. Encrypt data at rest
D. Improve query performance

**Answer:** B. Verify the identity of a user or application

**Reference:** Microsoft Learn – Authentication and Authorization

---

## Question 52

What is the primary purpose of authorization?

A. Verify identity
B. Determine permissions after authentication succeeds
C. Encrypt database files
D. Configure backups

**Answer:** B. Determine permissions after authentication succeeds

**Reference:** Microsoft Learn – Authentication and Authorization

---

## Question 53

Which security principal is typically used to group permissions for multiple users?

A. Schema
B. Role
C. Trigger
D. Constraint

**Answer:** B. Role

**Reference:** Microsoft Learn – Database-Level Roles

---

## Question 54

Which fixed database role provides full administrative control within a database?

A. db_datareader
B. db_datawriter
C. db_owner
D. public

**Answer:** C. db_owner

**Reference:** Microsoft Learn – Database-Level Roles

---

## Question 55

Which permission allows a user to retrieve data from a table?

A. EXECUTE
B. ALTER
C. SELECT
D. CONTROL

**Answer:** C. SELECT

**Reference:** Microsoft Learn – GRANT Object Permissions

---

## Question 56

Which statement is used to grant permissions to a user?

A. ALLOW
B. GRANT
C. AUTHORIZE
D. ENABLE

**Answer:** B. GRANT

**Reference:** Microsoft Learn – GRANT

---

## Question 57

Which statement explicitly removes a granted permission?

A. DELETE PERMISSION
B. DENY
C. REMOVE
D. DROP ACCESS

**Answer:** B. DENY

**Explanation:** DENY explicitly blocks access even when permissions might otherwise be inherited.

**Reference:** Microsoft Learn – DENY

---

## Question 58

What is the principle of least privilege?

A. Grant all permissions by default
B. Grant only the permissions necessary to perform required tasks
C. Use only Windows authentication
D. Disable auditing

**Answer:** B. Grant only the permissions necessary to perform required tasks

**Reference:** Microsoft Learn – Security Best Practices

---

## Question 59

What is the primary purpose of Row-Level Security (RLS)?

A. Encrypt data at rest
B. Restrict access to specific rows based on user context
C. Compress data
D. Track historical changes

**Answer:** B. Restrict access to specific rows based on user context

**Reference:** Microsoft Learn – Row-Level Security

---

## Question 60

Which object is commonly used by Row-Level Security to filter accessible rows?

A. Scalar Function
B. Security Policy with Predicate Function
C. Trigger
D. Sequence

**Answer:** B. Security Policy with Predicate Function

**Reference:** Microsoft Learn – Row-Level Security

---

## Question 61

What is the primary purpose of Dynamic Data Masking (DDM)?

A. Encrypt data permanently
B. Hide sensitive information from non-privileged users
C. Improve query performance
D. Archive data

**Answer:** B. Hide sensitive information from non-privileged users

**Reference:** Microsoft Learn – Dynamic Data Masking

---

## Question 62

Which statement about Dynamic Data Masking is true?

A. Data is encrypted in storage
B. Data is physically altered in the table
C. Data remains unchanged and only the displayed value is masked
D. DDM replaces Always Encrypted

**Answer:** C. Data remains unchanged and only the displayed value is masked

**Reference:** Microsoft Learn – Dynamic Data Masking

---

## Question 63

Which feature encrypts sensitive data so that SQL Server cannot see plaintext values?

A. TDE
B. DDM
C. Always Encrypted
D. Row-Level Security

**Answer:** C. Always Encrypted

**Reference:** Microsoft Learn – Always Encrypted

---

## Question 64

Where are encryption keys typically stored for Always Encrypted?

A. Database tables only
B. Client-side trusted key store
C. Query Store
D. TempDB

**Answer:** B. Client-side trusted key store

**Reference:** Microsoft Learn – Always Encrypted Key Management

---

## Question 65

What is the primary purpose of Transparent Data Encryption (TDE)?

A. Protect data in transit
B. Protect database files at rest
C. Restrict row access
D. Mask query results

**Answer:** B. Protect database files at rest

**Reference:** Microsoft Learn – Transparent Data Encryption

---

## Question 66

Which security feature protects backup files and database files if storage media is stolen?

A. Dynamic Data Masking
B. Row-Level Security
C. Transparent Data Encryption
D. Security Policies

**Answer:** C. Transparent Data Encryption

**Reference:** Microsoft Learn – Transparent Data Encryption

---

## Question 67

Which Azure SQL feature records database activities for compliance and investigation purposes?

A. Query Store
B. SQL Auditing
C. Columnstore Indexes
D. Temporal Tables

**Answer:** B. SQL Auditing

**Reference:** Microsoft Learn – SQL Auditing

---

## Question 68

What information is commonly captured by SQL Auditing?

A. Query execution plans only
B. Security-relevant events and database activities
C. Index fragmentation only
D. Backup schedules only

**Answer:** B. Security-relevant events and database activities

**Reference:** Microsoft Learn – SQL Auditing

---

## Question 69

What is a primary benefit of using Managed Identity with Azure SQL-related services?

A. Faster query execution
B. Eliminates the need to store credentials in application code
C. Reduces database size
D. Automatically creates indexes

**Answer:** B. Eliminates the need to store credentials in application code

**Reference:** Microsoft Learn – Managed Identities for Azure Resources

---

## Question 70

Why is passwordless authentication recommended when supported?

A. It reduces database storage costs
B. It improves indexing performance
C. It reduces risks associated with password theft and management
D. It replaces authorization

**Answer:** C. It reduces risks associated with password theft and management

**Reference:** Microsoft Learn – Passwordless Authentication Guidance

---

## DP-800 Exam Tips for Security

### Know the differences

| Feature              | Purpose                            |
| -------------------- | ---------------------------------- |
| Row-Level Security   | Restrict rows returned             |
| Dynamic Data Masking | Hide displayed values              |
| Always Encrypted     | Protect data from DB engine access |
| TDE                  | Protect data at rest               |
| Auditing             | Track activities                   |
| Managed Identity     | Eliminate stored credentials       |

### Frequently Tested Scenarios

**If the requirement is...**

* "Users should only see their own records" → **RLS**
* "Hide SSN except last four digits" → **DDM**
* "DBA must not see plaintext values" → **Always Encrypted**
* "Protect database files and backups" → **TDE**
* "Track who modified sensitive tables" → **SQL Auditing**
* "Application should authenticate without secrets" → **Managed Identity**

### Score Guide

* 18–20 Correct: Exam Ready
* 15–17 Correct: Strong Understanding
* 12–14 Correct: Review Encryption & RLS
* Below 12: Revisit Security Objectives
