# Database Isolation Levels

## Introduction

Isolation levels in DBMS define how transactions interact with each other when they are executed concurrently.

Isolation is one of the ACID properties. It ensures that transactions do not interfere with each other in a way that causes data inconsistency.

Different isolation levels provide different degrees of protection and performance.

---

## Why Isolation Levels are Important

Isolation levels help in:

- Preventing data inconsistency
- Controlling concurrency issues
- Managing transaction conflicts
- Balancing performance and accuracy

Higher isolation increases consistency but may reduce performance.

---

## Common Concurrency Problems

Isolation levels are designed to prevent these issues:

- Dirty Read
- Non-Repeatable Read
- Phantom Read

---

## 1. Dirty Read

- Occurs when a transaction reads uncommitted data from another transaction
- If the other transaction rolls back, the data becomes invalid
- Leads to incorrect results

---

## 2. Non-Repeatable Read

- Occurs when the same query returns different results within the same transaction
- Happens if another transaction modifies the data

---

## 3. Phantom Read

- Occurs when new rows are added or removed by another transaction
- Re-executing the same query returns additional or missing rows

---

## Types of Isolation Levels

There are four standard isolation levels:

- Read Uncommitted
- Read Committed
- Repeatable Read
- Serializable

---

## 1. Read Uncommitted

- Lowest isolation level
- Allows dirty reads
- High performance
- Least data protection

---

## 2. Read Committed

- Prevents dirty reads
- Only committed data can be read
- Moderate performance
- Still allows non-repeatable and phantom reads

---

## 3. Repeatable Read

- Prevents dirty reads
- Prevents non-repeatable reads
- May allow phantom reads
- Higher consistency

---

## 4. Serializable

- Highest isolation level
- Prevents dirty reads, non-repeatable reads, and phantom reads
- Ensures complete isolation
- Lowest performance due to strict locking
