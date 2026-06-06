# DP-800 Practice Question Bank

## Part 4 – Performance Optimization (Questions 71–90)

> References are based on Microsoft Learn / Microsoft Docs topics covered by the DP-800 study guide.

---

## Question 71

What is the primary purpose of Query Store?

A. Encrypt queries before execution
B. Capture query history, execution plans, and runtime statistics
C. Manage database backups
D. Store application logs

**Answer:** B. Capture query history, execution plans, and runtime statistics

**Reference:** Microsoft Learn – Query Store

---

## Question 72

Which problem is Query Store particularly useful for identifying?

A. Missing backups
B. Query performance regressions
C. Corrupted indexes only
D. Network failures

**Answer:** B. Query performance regressions

**Reference:** Microsoft Learn – Monitor Performance by Using Query Store

---

## Question 73

What is an execution plan?

A. A backup strategy document
B. A description of how SQL Server processes a query
C. A security configuration file
D. A deployment script

**Answer:** B. A description of how SQL Server processes a query

**Reference:** Microsoft Learn – Execution Plans

---

## Question 74

Which execution plan type shows the actual runtime metrics collected during query execution?

A. Estimated Execution Plan
B. Actual Execution Plan
C. Logical Execution Plan
D. Query Store Plan

**Answer:** B. Actual Execution Plan

**Reference:** Microsoft Learn – Display an Actual Execution Plan

---

## Question 75

Which execution plan type can be generated without running the query?

A. Actual Plan
B. Runtime Plan
C. Estimated Execution Plan
D. Query Statistics Plan

**Answer:** C. Estimated Execution Plan

**Reference:** Microsoft Learn – Display the Estimated Execution Plan

---

## Question 76

What does a table scan generally indicate?

A. SQL Server reads every row in a table
B. Data is encrypted
C. The query uses a clustered index efficiently
D. The query is blocked

**Answer:** A. SQL Server reads every row in a table

**Reference:** Microsoft Learn – Execution Plan Operators

---

## Question 77

Which operator usually indicates a more selective and efficient lookup than a scan?

A. Table Scan
B. Index Seek
C. Hash Warning
D. Sort

**Answer:** B. Index Seek

**Reference:** Microsoft Learn – Execution Plan Operators

---

## Question 78

What is a DMV?

A. Dynamic Management View
B. Database Monitoring Variable
C. Distributed Metadata View
D. Dynamic Memory Validator

**Answer:** A. Dynamic Management View

**Reference:** Microsoft Learn – Dynamic Management Views and Functions

---

## Question 79

Which DMV category is commonly used to investigate query performance?

A. sys.dm_exec_* views
B. sys.backup_* views
C. sys.email_* views
D. sys.login_* views only

**Answer:** A. sys.dm_exec_* views

**Reference:** Microsoft Learn – Query Performance DMVs

---

## Question 80

What is the purpose of Query Performance Insight in Azure SQL?

A. Create backups automatically
B. Visualize and identify resource-consuming queries
C. Encrypt execution plans
D. Configure auditing

**Answer:** B. Visualize and identify resource-consuming queries

**Reference:** Microsoft Learn – Query Performance Insight

---

## Question 81

What is blocking?

A. Data encryption process
B. One session preventing another session from accessing required resources
C. Index fragmentation
D. Backup compression

**Answer:** B. One session preventing another session from accessing required resources

**Reference:** Microsoft Learn – Understand and Resolve Blocking Problems

---

## Question 82

Which SQL Server mechanism typically causes blocking?

A. Locks
B. Sequences
C. Views
D. Triggers

**Answer:** A. Locks

**Reference:** Microsoft Learn – SQL Server Locking Architecture

---

## Question 83

What is a deadlock?

A. A failed backup operation
B. A circular dependency where sessions wait indefinitely on each other
C. An index rebuild process
D. A type of table scan

**Answer:** B. A circular dependency where sessions wait indefinitely on each other

**Reference:** Microsoft Learn – Deadlocks Guide

---

## Question 84

How does SQL Server resolve a deadlock?

A. Restarts the database
B. Terminates one transaction as the deadlock victim
C. Drops conflicting indexes
D. Pauses all queries

**Answer:** B. Terminates one transaction as the deadlock victim

**Reference:** Microsoft Learn – Deadlocks Guide

---

## Question 85

What is the purpose of transaction isolation levels?

A. Manage authentication
B. Control concurrency and data consistency behavior between transactions
C. Configure backups
D. Encrypt tables

**Answer:** B. Control concurrency and data consistency behavior between transactions

**Reference:** Microsoft Learn – Transaction Isolation Levels

---

## Question 86

Which isolation level provides the highest degree of isolation?

A. READ UNCOMMITTED
B. READ COMMITTED
C. REPEATABLE READ
D. SERIALIZABLE

**Answer:** D. SERIALIZABLE

**Reference:** Microsoft Learn – Transaction Isolation Levels

---

## Question 87

Which isolation level permits dirty reads?

A. SERIALIZABLE
B. SNAPSHOT
C. READ COMMITTED
D. READ UNCOMMITTED

**Answer:** D. READ UNCOMMITTED

**Reference:** Microsoft Learn – Transaction Isolation Levels

---

## Question 88

What is index fragmentation?

A. Missing security permissions
B. Inefficient organization of index pages that can affect performance
C. Data corruption
D. Deadlock occurrence

**Answer:** B. Inefficient organization of index pages that can affect performance

**Reference:** Microsoft Learn – Reorganize and Rebuild Indexes

---

## Question 89

When fragmentation becomes significant, which maintenance operation is commonly used?

A. CREATE USER
B. REBUILD INDEX
C. BACKUP LOG
D. CREATE VIEW

**Answer:** B. REBUILD INDEX

**Reference:** Microsoft Learn – Reorganize and Rebuild Indexes

---

## Question 90

A query suddenly becomes slower after a deployment even though the data has not changed significantly. Which tool should be investigated first?

A. Query Store
B. Dynamic Data Masking
C. Temporal Tables
D. SQL Auditing

**Answer:** A. Query Store

**Explanation:** Query Store is specifically designed to identify query plan changes and performance regressions.

**Reference:** Microsoft Learn – Query Store

---

## DP-800 Performance Optimization Cheat Sheet

### Execution Plans

| Operator             | Usually Good?     |
| -------------------- | ----------------- |
| Index Seek           | ✅ Preferred       |
| Key Lookup           | ⚠️ Depends        |
| Clustered Index Scan | ⚠️ Review         |
| Table Scan           | ❌ Often expensive |

---

### Blocking vs Deadlock

| Concept    | Description                          |
| ---------- | ------------------------------------ |
| Blocking   | One session waits                    |
| Deadlock   | Sessions wait on each other          |
| Resolution | SQL Server chooses a deadlock victim |

---

### Isolation Levels

| Level            | Dirty Reads |
| ---------------- | ----------- |
| READ UNCOMMITTED | Yes         |
| READ COMMITTED   | No          |
| REPEATABLE READ  | No          |
| SERIALIZABLE     | No          |

---

### Common DP-800 Scenario Questions

**Performance regression after deployment**
→ Query Store

**Identify expensive queries**
→ Query Performance Insight / DMVs

**Investigate query execution strategy**
→ Execution Plan

**Excessive waits between sessions**
→ Blocking Analysis

**Circular waiting transactions**
→ Deadlock Analysis

**Maintain heavily fragmented indexes**
→ Rebuild or Reorganize Indexes

---

### Score Guide

* 18–20 Correct: Exam Ready
* 15–17 Correct: Strong Understanding
* 12–14 Correct: Review Query Store & Concurrency
* Below 12: Revisit Performance Objectives
