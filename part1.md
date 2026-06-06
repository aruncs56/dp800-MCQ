# DP-800 Practice Question Bank

## Part 1 – Design and Develop Database Solutions (Questions 1–25)

> References are from Microsoft Learn / Microsoft Docs and align with the DP-800 study guide objectives.

---

## Question 1

Which constraint ensures that each row in a table can be uniquely identified and does not allow NULL values?

A. UNIQUE
B. CHECK
C. PRIMARY KEY
D. DEFAULT

**Answer:** C. PRIMARY KEY

**Explanation:** A PRIMARY KEY uniquely identifies each row in a table and automatically enforces uniqueness and NOT NULL behavior.

**Reference:** Microsoft Learn – Primary and Foreign Key Constraints

---

## Question 2

What is the primary purpose of a FOREIGN KEY constraint?

A. Encrypt data between tables
B. Maintain referential integrity between tables
C. Improve query performance
D. Prevent duplicate values

**Answer:** B. Maintain referential integrity between tables

**Explanation:** FOREIGN KEY constraints ensure relationships between parent and child tables remain valid.

**Reference:** Microsoft Learn – Primary and Foreign Key Constraints

---

## Question 3

Which constraint restricts values in a column to meet a specified condition?

A. CHECK
B. UNIQUE
C. DEFAULT
D. INDEX

**Answer:** A. CHECK

**Explanation:** CHECK constraints enforce domain integrity by validating data against a logical expression.

**Reference:** Microsoft Learn – Create CHECK Constraints

---

## Question 4

What happens when a UNIQUE constraint is applied to a column?

A. Duplicate values are allowed
B. Only numeric values are permitted
C. Duplicate values are prevented
D. Values are encrypted

**Answer:** C. Duplicate values are prevented

**Explanation:** UNIQUE constraints ensure no duplicate values exist within the constrained column(s).

**Reference:** Microsoft Learn – Unique Constraints and Check Constraints

---

## Question 5

Which object can automatically generate sequential numeric values independent of a table?

A. Trigger
B. Sequence
C. Cursor
D. View

**Answer:** B. Sequence

**Explanation:** A sequence object generates ordered numeric values that can be used across multiple tables.

**Reference:** Microsoft Learn – Sequence Numbers

---

## Question 6

Which index type physically determines the storage order of rows in a table?

A. XML Index
B. Full-Text Index
C. Clustered Index
D. Spatial Index

**Answer:** C. Clustered Index

**Explanation:** A clustered index sorts and stores data rows according to the index key.

**Reference:** Microsoft Learn – Clustered and Nonclustered Indexes

---

## Question 7

How many clustered indexes can a table have?

A. Unlimited
B. One
C. Two
D. Ten

**Answer:** B. One

**Explanation:** Since data rows can be physically ordered only one way, a table can have only one clustered index.

**Reference:** Microsoft Learn – Clustered and Nonclustered Indexes

---

## Question 8

What is the primary benefit of a nonclustered index?

A. Encrypts data
B. Stores historical versions of rows
C. Improves query performance for searches and lookups
D. Automatically partitions data

**Answer:** C. Improves query performance for searches and lookups

**Explanation:** Nonclustered indexes provide alternate access paths to data without changing physical row order.

**Reference:** Microsoft Learn – Clustered and Nonclustered Indexes

---

## Question 9

Which index type is optimized for analytical workloads involving large-scale aggregations?

A. Full-Text Index
B. Spatial Index
C. XML Index
D. Columnstore Index

**Answer:** D. Columnstore Index

**Explanation:** Columnstore indexes store data by column and significantly improve analytics performance.

**Reference:** Microsoft Learn – Columnstore Indexes

---

## Question 10

What is a key characteristic of a system-versioned temporal table?

A. Stores JSON documents only
B. Tracks full history of data changes automatically
C. Requires triggers for versioning
D. Supports graph relationships

**Answer:** B. Tracks full history of data changes automatically

**Explanation:** Temporal tables automatically maintain current and historical versions of rows.

**Reference:** Microsoft Learn – Temporal Tables

---

## Question 11

A temporal table requires which additional object?

A. History table
B. Graph node table
C. External data source
D. Ledger view

**Answer:** A. History table

**Explanation:** SQL Server stores previous row versions in an associated history table.

**Reference:** Microsoft Learn – Temporal Tables

---

## Question 12

What is the primary goal of a ledger table?

A. Improve indexing performance
B. Store graph relationships
C. Provide tamper-evident data integrity
D. Compress JSON documents

**Answer:** C. Provide tamper-evident data integrity

**Explanation:** Ledger tables help detect unauthorized modifications using cryptographic verification.

**Reference:** Microsoft Learn – Ledger Overview

---

## Question 13

Which table type is designed for graph data modeling?

A. Temporal Table
B. Ledger Table
C. Node Table
D. External Table

**Answer:** C. Node Table

**Explanation:** Graph databases in SQL Server use node and edge tables to represent entities and relationships.

**Reference:** Microsoft Learn – SQL Graph Architecture

---

## Question 14

What does an edge table represent in SQL Graph?

A. Historical versions
B. Relationships between entities
C. External datasets
D. Encrypted rows

**Answer:** B. Relationships between entities

**Explanation:** Edge tables define connections between node records.

**Reference:** Microsoft Learn – SQL Graph Architecture

---

## Question 15

What is an external table primarily used for?

A. Storing encrypted values
B. Accessing data stored outside SQL Server tables
C. Managing indexes
D. Creating views

**Answer:** B. Accessing data stored outside SQL Server tables

**Explanation:** External tables allow querying data stored externally through supported connectors.

**Reference:** Microsoft Learn – External Tables

---

## Question 16

Which SQL Server feature is optimized for high-throughput OLTP workloads using memory-optimized structures?

A. Full-Text Search
B. In-Memory OLTP
C. Temporal Tables
D. Ledger

**Answer:** B. In-Memory OLTP

**Explanation:** In-Memory OLTP improves transaction processing performance using memory-optimized tables.

**Reference:** Microsoft Learn – In-Memory OLTP Overview

---

## Question 17

Which JSON function extracts a scalar value from JSON data?

A. JSON_QUERY
B. OPENJSON
C. JSON_VALUE
D. STRING_SPLIT

**Answer:** C. JSON_VALUE

**Explanation:** JSON_VALUE returns a scalar value from a specified JSON path.

**Reference:** Microsoft Learn – JSON Functions

---

## Question 18

Which JSON function returns an object or array from JSON text?

A. JSON_VALUE
B. JSON_QUERY
C. FORMAT
D. PARSE

**Answer:** B. JSON_QUERY

**Explanation:** JSON_QUERY returns JSON objects or arrays rather than scalar values.

**Reference:** Microsoft Learn – JSON Functions

---

## Question 19

Which function converts JSON text into relational rows and columns?

A. OPENJSON
B. JSON_VALUE
C. CONCAT
D. FORMATMESSAGE

**Answer:** A. OPENJSON

**Explanation:** OPENJSON parses JSON data into a tabular format.

**Reference:** Microsoft Learn – OPENJSON

---

## Question 20

Why would you create an index on a JSON property?

A. Encrypt JSON documents
B. Improve performance of JSON-based queries
C. Validate JSON schema
D. Enable temporal tracking

**Answer:** B. Improve performance of JSON-based queries

**Explanation:** Indexed computed columns based on JSON values can significantly improve query performance.

**Reference:** Microsoft Learn – Index JSON Data

---

## Question 21

What is the purpose of horizontal table partitioning?

A. Encrypt rows separately
B. Divide data into manageable segments based on a partition key
C. Create backups automatically
D. Reduce column count

**Answer:** B. Divide data into manageable segments based on a partition key

**Explanation:** Partitioning improves manageability and can enhance query performance.

**Reference:** Microsoft Learn – Table and Index Partitioning

---

## Question 22

Which object defines how rows are distributed among partitions?

A. Partition Function
B. Trigger
C. Sequence
D. View

**Answer:** A. Partition Function

**Explanation:** A partition function maps row values to partitions.

**Reference:** Microsoft Learn – Partitioned Tables and Indexes

---

## Question 23

Which object maps partitions to filegroups?

A. Partition Scheme
B. Constraint
C. Sequence
D. Ledger View

**Answer:** A. Partition Scheme

**Explanation:** A partition scheme associates partitions with storage locations.

**Reference:** Microsoft Learn – Partitioned Tables and Indexes

---

## Question 24

Which table feature is specifically designed to provide cryptographic verification of data changes?

A. Temporal Table
B. External Table
C. Ledger Table
D. Node Table

**Answer:** C. Ledger Table

**Explanation:** Ledger tables help establish trust by making data modifications tamper-evident.

**Reference:** Microsoft Learn – Ledger Overview

---

## Question 25

You need to store application configuration data as flexible key-value pairs and query specific attributes efficiently. Which SQL Server capability best supports this requirement?

A. Graph Tables
B. JSON Support with Indexed Properties
C. Temporal Tables
D. Ledger Tables

**Answer:** B. JSON Support with Indexed Properties

**Explanation:** SQL Server supports storing semi-structured JSON data while enabling efficient access through indexed computed columns.

**Reference:** Microsoft Learn – JSON Data in SQL Server

---

### Score Guide

* 23–25 Correct: Exam Ready
* 20–22 Correct: Strong Understanding
* 16–19 Correct: Review Weak Areas
* Below 16: Revisit Design & Development Objectives

Next, I recommend creating **Part 2 – Programmability & Advanced T-SQL (25 questions)** because it is one of the highest-weighted and most tested areas in DP-800.
