# DP-800 Practice Question Bank

## Part 2 – Programmability & Advanced T-SQL (Questions 26–50)

> References are based on Microsoft Learn / Microsoft Docs topics covered by the DP-800 study guide.

---

## Question 26

Which database object stores a reusable SELECT statement that can be queried like a table?

A. Stored Procedure
B. View
C. Trigger
D. Sequence

**Answer:** B. View

**Explanation:** A view is a virtual table based on the result set of a SELECT statement.

**Reference:** Microsoft Learn – CREATE VIEW

---

## Question 27

What is a primary benefit of using a view?

A. Encrypts data automatically
B. Simplifies complex queries and restricts data exposure
C. Improves backup speed
D. Creates indexes automatically

**Answer:** B. Simplifies complex queries and restricts data exposure

**Reference:** Microsoft Learn – Views

---

## Question 28

Which object can accept parameters and return a single scalar value?

A. Table-Valued Function
B. View
C. Scalar Function
D. Trigger

**Answer:** C. Scalar Function

**Explanation:** Scalar functions return a single value of a specified data type.

**Reference:** Microsoft Learn – User-Defined Functions

---

## Question 29

Which type of function returns a table result?

A. Scalar Function
B. Aggregate Function
C. Table-Valued Function
D. Trigger Function

**Answer:** C. Table-Valued Function

**Reference:** Microsoft Learn – Table-Valued Functions

---

## Question 30

What is the main purpose of a stored procedure?

A. Store query execution plans permanently
B. Encapsulate reusable SQL logic that can be executed as a unit
C. Create indexes automatically
D. Replace database backups

**Answer:** B. Encapsulate reusable SQL logic that can be executed as a unit

**Reference:** Microsoft Learn – Stored Procedures

---

## Question 31

Which statement executes a stored procedure?

A. RUN
B. EXEC
C. START
D. CALLPROC

**Answer:** B. EXEC

**Reference:** Microsoft Learn – Execute Stored Procedures

---

## Question 32

When is a DML trigger executed?

A. When a database starts
B. In response to INSERT, UPDATE, or DELETE operations
C. During backup operations
D. During index creation

**Answer:** B. In response to INSERT, UPDATE, or DELETE operations

**Reference:** Microsoft Learn – DML Triggers

---

## Question 33

Which pseudo-table contains new row values within a trigger?

A. CURRENT
B. UPDATED
C. INSERTED
D. CHANGED

**Answer:** C. INSERTED

**Reference:** Microsoft Learn – Use INSERTED and DELETED Tables

---

## Question 34

Which pseudo-table contains old row values during UPDATE and DELETE operations?

A. PREVIOUS
B. DELETED
C. HISTORY
D. OLDROWS

**Answer:** B. DELETED

**Reference:** Microsoft Learn – Use INSERTED and DELETED Tables

---

## Question 35

What is a Common Table Expression (CTE)?

A. A temporary named result set defined within a query
B. A permanent database object
C. A type of index
D. A security feature

**Answer:** A. A temporary named result set defined within a query

**Reference:** Microsoft Learn – WITH Common Table Expression

---

## Question 36

Which keyword begins a CTE definition?

A. TEMP
B. CTE
C. WITH
D. DEFINE

**Answer:** C. WITH

**Reference:** Microsoft Learn – WITH Common Table Expression

---

## Question 37

Which T-SQL feature allows a query to reference itself recursively?

A. Cursor
B. Recursive CTE
C. Trigger
D. Sequence

**Answer:** B. Recursive CTE

**Reference:** Microsoft Learn – Recursive Queries Using CTEs

---

## Question 38

Which window function assigns a unique sequential number to rows?

A. DENSE_RANK()
B. ROW_NUMBER()
C. COUNT()
D. AVG()

**Answer:** B. ROW_NUMBER()

**Reference:** Microsoft Learn – ROW_NUMBER

---

## Question 39

What is the difference between RANK() and DENSE_RANK()?

A. No difference
B. DENSE_RANK() does not leave gaps after ties
C. RANK() is faster
D. RANK() works only on integers

**Answer:** B. DENSE_RANK() does not leave gaps after ties

**Reference:** Microsoft Learn – Ranking Functions

---

## Question 40

Which clause is required by most window functions?

A. PARTITION BY or ORDER BY within OVER()
B. GROUP BY
C. HAVING
D. COMPUTE

**Answer:** A. PARTITION BY or ORDER BY within OVER()

**Reference:** Microsoft Learn – OVER Clause

---

## Question 41

Which function returns the previous row value within a result set?

A. PREV()
B. PRIOR()
C. LAG()
D. BEFORE()

**Answer:** C. LAG()

**Reference:** Microsoft Learn – LAG

---

## Question 42

Which function returns the next row value within a result set?

A. NEXTROW()
B. LEAD()
C. FOLLOW()
D. ADVANCE()

**Answer:** B. LEAD()

**Reference:** Microsoft Learn – LEAD

---

## Question 43

What is a correlated subquery?

A. A subquery executed only once
B. A subquery that references columns from the outer query
C. A recursive query
D. A stored procedure call

**Answer:** B. A subquery that references columns from the outer query

**Reference:** Microsoft Learn – Subqueries

---

## Question 44

Which construct is commonly used to handle runtime errors in T-SQL?

A. ON ERROR
B. HANDLE ERROR
C. TRY...CATCH
D. EXCEPTION

**Answer:** C. TRY...CATCH

**Reference:** Microsoft Learn – TRY...CATCH

---

## Question 45

Which function returns the error message within a CATCH block?

A. ERROR_TEXT()
B. ERROR_MESSAGE()
C. GET_ERROR()
D. LAST_ERROR()

**Answer:** B. ERROR_MESSAGE()

**Reference:** Microsoft Learn – ERROR_MESSAGE

---

## Question 46

Which JSON function returns a scalar value from JSON text?

A. OPENJSON
B. JSON_QUERY
C. JSON_VALUE
D. JSON_PARSE

**Answer:** C. JSON_VALUE

**Reference:** Microsoft Learn – JSON Functions

---

## Question 47

Which JSON function returns a JSON object or array?

A. JSON_QUERY
B. JSON_VALUE
C. OPENROWSET
D. STRING_SPLIT

**Answer:** A. JSON_QUERY

**Reference:** Microsoft Learn – JSON Functions

---

## Question 48

Which function transforms JSON data into rows and columns?

A. JSON_TABLE
B. JSON_VALUE
C. OPENJSON
D. PARSEJSON

**Answer:** C. OPENJSON

**Reference:** Microsoft Learn – OPENJSON

---

## Question 49

Why are window functions often preferred over self-joins for analytical calculations?

A. They automatically encrypt results
B. They simplify calculations and can improve readability and performance
C. They eliminate indexes
D. They require less memory in all scenarios

**Answer:** B. They simplify calculations and can improve readability and performance

**Reference:** Microsoft Learn – Query Processing with Window Functions

---

## Question 50

A developer needs to calculate a running total of sales ordered by transaction date. Which feature is most appropriate?

A. Trigger
B. Cursor
C. Window Aggregate Function using OVER()
D. Foreign Key

**Answer:** C. Window Aggregate Function using OVER()

**Explanation:** Window aggregates such as SUM() OVER() are commonly used for running totals and analytical calculations.

**Reference:** Microsoft Learn – OVER Clause and Window Aggregates

---

### Score Guide

* 23–25 Correct: DP-800 Ready for T-SQL Objectives
* 20–22 Correct: Strong Understanding
* 16–19 Correct: Review CTEs, Window Functions, and Error Handling
* Below 16: Revisit Programmability and Advanced Querying Topics
