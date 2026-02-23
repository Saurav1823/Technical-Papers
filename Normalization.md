# Normalization in Database

## Introduction

Normalization is the process of organizing data in a database to reduce redundancy and improve data integrity.

It involves dividing large tables into smaller related tables and defining relationships between them.

Normalization is mainly used in relational database design.

---

## Why Normalization is Important

Normalization helps in:

- Reducing data duplication
- Preventing data anomalies
- Improving data consistency
- Making database structure more organized

Without normalization, databases may contain repeated and inconsistent data.

---

## Types of Data Anomalies

Normalization prevents the following anomalies:

- Insertion anomaly
- Update anomaly
- Deletion anomaly

These problems occur when data is not properly structured.

---

## Normal Forms

Normalization is divided into different levels called Normal Forms.

---

## 1. First Normal Form (1NF)

A table is in 1NF if:

- Each column contains atomic (single) values
- There are no repeating groups
- Each record is unique

---

## 2. Second Normal Form (2NF)

A table is in 2NF if:

- It is already in 1NF
- All non-key attributes are fully dependent on the primary key

This removes partial dependency.

---

## 3. Third Normal Form (3NF)

A table is in 3NF if:

- It is already in 2NF
- There is no transitive dependency
- Non-key attributes depend only on the primary key

This removes indirect dependency.

---

## Boyce-Codd Normal Form (BCNF)

BCNF is a stricter version of 3NF.

- Every determinant must be a candidate key
- Removes certain types of anomalies not handled by 3NF

---

## Advantages of Normalization

- Reduces data redundancy
- Improves data consistency
- Prevents modification anomalies
- Enhances database structure
- Makes maintenance easier

---
