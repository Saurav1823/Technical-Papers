# Triggers 

## Introduction

A Trigger in DBMS is a special type of stored procedure that automatically executes in response to certain events on a table or view.

Triggers are used to enforce rules, maintain data integrity, and automate tasks inside the database.

They are activated automatically when a specified event occurs.

---

## Why Triggers are Important

Triggers help in:

- Enforcing business rules
- Maintaining data integrity
- Auditing changes
- Automating repetitive tasks
- Preventing invalid data operations

They ensure that certain actions happen automatically when data changes.

---

## Events That Activate Triggers

Triggers are generally activated by the following events:

- INSERT
- UPDATE
- DELETE

These events occur when data is added, modified, or removed from a table.

---

## Types of Triggers

There are different types of triggers based on timing and level:

- BEFORE Trigger
- AFTER Trigger
- INSTEAD OF Trigger
- Row-Level Trigger
- Statement-Level Trigger

---

## 1. BEFORE Trigger

A BEFORE Trigger executes before the actual database operation.

- Used to validate data
- Can modify data before saving
- Prevents invalid entries

It is commonly used for validation purposes.

---

## 2. AFTER Trigger

An AFTER Trigger executes after the database operation is completed.

- Used for logging or auditing
- Ensures action occurs only after successful operation
- Cannot modify original operation result

---

## 3. INSTEAD OF Trigger

An INSTEAD OF Trigger replaces the original operation.

- Commonly used with views
- Customizes behavior of INSERT, UPDATE, or DELETE
- Executes alternative logic

---

## 4. Row-Level Trigger

- Executes once for each affected row
- Useful when individual row processing is needed
- More detailed control

---

## 5. Statement-Level Trigger

- Executes once for the entire SQL statement
- Does not depend on number of rows affected
- Used for general operations

---

## Advantages of Triggers

- Automates database operations
- Improves data consistency
- Enforces complex business rules
- Useful for auditing and logging

---
