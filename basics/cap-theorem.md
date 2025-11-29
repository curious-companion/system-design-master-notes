# CAP Theorem

CAP Theorem says that in a distributed system, you can only guarantee **two** of the following three consistently:

- **C – Consistency**  
  Every read gets the latest write.

- **A – Availability**  
  System always responds (even if outdated).

- **P – Partition Tolerance**  
  System continues working even if network splits occur.

---

## Why Partition Tolerance Is Mandatory

All distributed systems face network issues →  
So real-world systems must tolerate partitions (P).

Thus, systems choose between:

- **CP (Consistency + Partition Tolerance)**  
  - Might reject requests  
  - Example: MongoDB (in some modes), HBase  

- **AP (Availability + Partition Tolerance)**  
  - Always responds, but may return stale data  
  - Example: Cassandra, DynamoDB  

---

## Interview Shortcut

- If correctness > availability → **CP**  
- If availability > correctness → **AP**

---

## Summary

You cannot have **Consistency + Availability + Partition Tolerance** at the same time.  
Distributed systems must sacrifice one (usually Availability or Consistency).
