# Transactions in DBMS

## Introduction

A transaction in a Database Management System (DBMS) is a sequence of operations performed as a single logical unit of work.

A transaction ensures that database operations are completed fully and correctly. If any part of the transaction fails, the entire operation is rolled back.

Transactions are essential for maintaining data integrity and consistency.

---

## Why Transactions are Important

Transactions help in:

- Maintaining data consistency
- Preventing partial updates
- Handling system failures safely
- Supporting concurrent user operations

They ensure reliable processing of database operations.

---

## Characteristics of a Transaction

A transaction typically includes:

- Read operation
- Write operation
- Commit operation
- Rollback operation

These operations together ensure proper execution and recovery.

---

## Transaction States

A transaction passes through different states during execution:

- Active
- Partially Committed
- Committed
- Failed
- Aborted

---

## 1. Active State

- The transaction is currently executing.
- Database operations are being performed.

---

## 2. Partially Committed State

- All operations are executed.
- Waiting for final confirmation to make changes permanent.

---

## 3. Committed State

- All operations are successfully completed.
- Changes are permanently saved in the database.

---

## 4. Failed State

- An error occurs during execution.
- The transaction cannot continue.

---

## 5. Aborted State

- The transaction is rolled back.
- Database is restored to its previous consistent state.

---

## Properties of Transactions

Transactions follow the ACID properties:

- Atomicity
- Consistency
- Isolation
- Durability

These properties guarantee safe and reliable transaction processing.

---

## Advantages of Transactions

- Prevents data corruption
- Ensures data reliability
- Supports multi-user environments
- Enables safe recovery after failures

---

