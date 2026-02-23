# Indexes in DBMS

## Introduction

An index in a Database Management System is a data structure used to improve the speed of data retrieval operations on a table.

Indexes work similarly to an index in a book. Instead of scanning the entire table, the database uses the index to quickly locate the required data.

---

## Why Indexes are Important

Indexes help in:

- Speeding up data retrieval
- Reducing query execution time
- Improving overall database performance
- Efficiently handling large datasets

Without indexes, the database must perform a full table scan, which becomes slow when the table contains a large number of records.

---

## How Indexes Work

An index stores:

- Indexed column values
- A reference (pointer) to the actual row in the table

When a query searches for a specific value, the database first checks the index structure. Once the value is found in the index, it directly accesses the corresponding row in the table.

Most databases internally use tree-based structures like B-Trees to maintain indexes efficiently.

---

## Types of Indexes

There are different types of indexes used in DBMS:

- Primary Index
- Secondary Index
- Unique Index
- Composite Index
- Clustered Index
- Non-Clustered Index

---

## 1. Primary Index

A Primary Index is automatically created when a primary key is defined.

- Ensures each value is unique
- Does not allow NULL values
- Often used to uniquely identify each record
- In some systems, it determines the physical storage order of data

It is mainly used for fast lookup using the primary key.

---

## 2. Secondary Index

A Secondary Index is created on non-primary key columns.

- Can be created manually
- May contain duplicate values
- Improves search performance on non-key columns
- Does not affect physical order of data

It is useful when frequently searching by columns other than the primary key.

---

## 3. Unique Index

A Unique Index ensures that all values in the indexed column are unique.

- Prevents duplicate entries
- Allows fast validation of uniqueness
- Commonly used for email IDs, usernames, etc.

It helps maintain data integrity.

---

## 4. Composite Index

A Composite Index is created on two or more columns.

- Improves performance for multi-column queries
- Order of columns in the index matters
- Useful when queries frequently filter using multiple columns

It is commonly used in complex search conditions.

---

## 5. Clustered Index

A Clustered Index determines the physical order of data in a table.

- Data rows are stored according to the indexed column
- Only one clustered index is allowed per table
- Faster for range-based queries

Since data is physically sorted, retrieval becomes more efficient.

---

## 6. Non-Clustered Index

A Non-Clustered Index creates a separate structure from the actual data.

- Stores indexed values and pointers to rows
- Multiple non-clustered indexes can exist on a table
- Does not change physical order of data

It provides flexibility in searching different columns.

---

## Advantages of Indexes

- Faster data retrieval
- Improved query performance
- Efficient searching and sorting
- Better performance for large databases

---

## Disadvantages of Indexes

- Increases storage space
- Slows down insert, update, and delete operations
- Requires regular maintenance

---
