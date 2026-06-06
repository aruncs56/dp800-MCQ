# DP-800 Practice Question Bank

## Part 6 – Azure Integration (Questions 106–120)

> References are based on Microsoft Learn / Microsoft Docs topics covered by the DP-800 study guide.

---

## Question 106

What is the primary purpose of Data API Builder (DAB)?

A. Encrypt Azure SQL databases
B. Generate REST and GraphQL endpoints for database objects
C. Create execution plans
D. Monitor database performance

**Answer:** B. Generate REST and GraphQL endpoints for database objects

**Reference:** Microsoft Learn – Data API Builder for Azure Databases

---

## Question 107

Which API styles can Data API Builder expose?

A. SOAP only
B. REST only
C. REST and GraphQL
D. OData only

**Answer:** C. REST and GraphQL

**Reference:** Microsoft Learn – Data API Builder Overview

---

## Question 108

What is the primary benefit of Data API Builder?

A. Eliminates the need to manually build common data access APIs
B. Replaces SQL Server entirely
C. Creates backups automatically
D. Performs index tuning

**Answer:** A. Eliminates the need to manually build common data access APIs

**Reference:** Microsoft Learn – Data API Builder Overview

---

## Question 109

In a REST API, which HTTP method is commonly used to retrieve data?

A. POST
B. PUT
C. GET
D. DELETE

**Answer:** C. GET

**Reference:** Microsoft Learn – REST API Fundamentals

---

## Question 110

Which HTTP method is typically used to create a new resource?

A. GET
B. POST
C. DELETE
D. HEAD

**Answer:** B. POST

**Reference:** Microsoft Learn – REST API Fundamentals

---

## Question 111

What is a key advantage of GraphQL compared to traditional REST endpoints?

A. It automatically encrypts data
B. Clients can request exactly the data they need
C. It removes authentication requirements
D. It replaces SQL

**Answer:** B. Clients can request exactly the data they need

**Reference:** Microsoft Learn – GraphQL Concepts

---

## Question 112

Which Azure service is commonly used to execute serverless code in response to events?

A. Azure Functions
B. Azure SQL Database
C. Azure Key Vault
D. Azure DevOps

**Answer:** A. Azure Functions

**Reference:** Microsoft Learn – Azure Functions Overview

---

## Question 113

What is a common use case for Azure Functions with Azure SQL?

A. Managing clustered indexes
B. Responding to events and automating workflows
C. Replacing database backups
D. Creating execution plans

**Answer:** B. Responding to events and automating workflows

**Reference:** Microsoft Learn – Azure Functions Integration Scenarios

---

## Question 114

What is Change Data Capture (CDC)?

A. A backup strategy
B. A feature that records insert, update, and delete activity for tracked tables
C. An encryption method
D. An indexing strategy

**Answer:** B. A feature that records insert, update, and delete activity for tracked tables

**Reference:** Microsoft Learn – Change Data Capture

---

## Question 115

What is a primary use case for CDC?

A. Tracking data modifications for downstream systems and analytics
B. Managing user authentication
C. Rebuilding indexes
D. Encrypting tables

**Answer:** A. Tracking data modifications for downstream systems and analytics

**Reference:** Microsoft Learn – Change Data Capture

---

## Question 116

How does Change Tracking differ from CDC?

A. Change Tracking captures full row history
B. CDC and Change Tracking are identical
C. Change Tracking identifies changed rows but stores less detailed information than CDC
D. Change Tracking requires GraphQL

**Answer:** C. Change Tracking identifies changed rows but stores less detailed information than CDC

**Reference:** Microsoft Learn – Change Tracking vs CDC

---

## Question 117

Which feature would generally be preferred when a consumer needs details of data modifications, including operation type?

A. Dynamic Data Masking
B. Change Tracking
C. Change Data Capture
D. Query Store

**Answer:** C. Change Data Capture

**Reference:** Microsoft Learn – CDC Overview

---

## Question 118

What is Azure Monitor primarily used for?

A. Version control management
B. Collecting, analyzing, and acting on telemetry data
C. Creating database schemas
D. Managing SQL permissions

**Answer:** B. Collecting, analyzing, and acting on telemetry data

**Reference:** Microsoft Learn – Azure Monitor Overview

---

## Question 119

Which type of information can Azure Monitor collect?

A. Metrics and logs
B. Only authentication events
C. Only backup information
D. Only execution plans

**Answer:** A. Metrics and logs

**Reference:** Microsoft Learn – Azure Monitor Overview

---

## Question 120

A solution requires exposing Azure SQL data through both REST and GraphQL endpoints while minimizing custom API development. Which technology best meets this requirement?

A. Query Store
B. Azure Key Vault
C. Data API Builder
D. SQL Auditing

**Answer:** C. Data API Builder

**Explanation:** Data API Builder can generate REST and GraphQL endpoints directly from database objects, reducing custom development effort.

**Reference:** Microsoft Learn – Data API Builder for Azure Databases

---

## DP-800 Azure Integration Cheat Sheet

### Integration Technologies

| Technology       | Purpose                           |
| ---------------- | --------------------------------- |
| Data API Builder | REST + GraphQL endpoints          |
| REST API         | Standard HTTP-based access        |
| GraphQL          | Flexible data retrieval           |
| Azure Functions  | Serverless processing             |
| CDC              | Detailed change capture           |
| Change Tracking  | Lightweight change identification |
| Azure Monitor    | Metrics and logs                  |

---

### CDC vs Change Tracking

| Feature                     | CDC | Change Tracking |
| --------------------------- | --- | --------------- |
| Tracks Inserts              | ✅   | ✅               |
| Tracks Updates              | ✅   | ✅               |
| Tracks Deletes              | ✅   | ✅               |
| Stores Detailed Change Info | ✅   | ❌               |
| Lightweight Sync Scenarios  | ⚠️  | ✅               |

---

### Common DP-800 Scenarios

**Need REST and GraphQL APIs quickly**
→ Data API Builder

**Need event-driven processing**
→ Azure Functions

**Need detailed record of data changes**
→ CDC

**Need lightweight synchronization**
→ Change Tracking

**Need centralized monitoring**
→ Azure Monitor

**Need application-specific data retrieval**
→ GraphQL

---

### Score Guide

* 14–15 Correct: Exam Ready
* 11–13 Correct: Strong Understanding
* 8–10 Correct: Review CDC, DAB, and Azure Monitor
* Below 8: Revisit Azure Integration Objectives
