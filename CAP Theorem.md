# CAP Theorem in Distributed Systems

## Introduction

CAP Theorem is a fundamental principle in distributed systems.  
It states that a distributed system can provide only two out of the following three guarantees at the same time:

- Consistency
- Availability
- Partition Tolerance

This theorem helps system designers understand trade-offs in distributed databases.

---

## What is CAP Theorem?

CAP stands for:

- C – Consistency
- A – Availability
- P – Partition Tolerance

According to the theorem, during a network partition, a system must choose between Consistency and Availability.

---

## 1. Consistency

Consistency means every read operation receives the most recent write.

If a data update happens, all nodes in the system must reflect that change immediately.

### Key Points

- All users see the same data at the same time
- No stale or outdated data is returned
- Similar to strong consistency in databases

---

## 2. Availability

Availability means every request receives a response, even if some nodes are down.

The system continues to operate and respond to users.

### Key Points

- System remains operational
- Every request gets a response
- Response may not always contain the latest data

---

## 3. Partition Tolerance

Partition Tolerance means the system continues to function even if communication between nodes is broken.

Network failures are common in distributed systems, so partition tolerance is essential.

### Key Points

- System works despite network failures
- Nodes may be unable to communicate temporarily
- Required for large distributed systems

---

## CAP Combinations

A distributed system can choose only two of the three properties:

- CP (Consistency + Partition Tolerance)
- AP (Availability + Partition Tolerance)
- CA (Consistency + Availability) – Not practical in real distributed systems when partitions occur

---

## Summary Table

| Property              | Meaning |
|-----------------------|----------|
| Consistency           | Same data across all nodes |
| Availability          | Every request gets a response |
| Partition Tolerance   | System works despite network failure |

---

## Conclusion

CAP Theorem explains the trade-offs in distributed systems.  
Since network failures are unavoidable, modern distributed systems usually choose between:

- Consistency and Partition Tolerance (CP systems)
- Availability and Partition Tolerance (AP systems)

Understanding CAP Theorem helps in designing scalable and reliable distributed databases.
