# Databases

Databases store and retrieve application data. Choosing the right type is key in system design.

---

## SQL Databases (Relational)

Examples: MySQL, PostgreSQL

- Strong consistency  
- Structured schema  
- Supports JOINs  
- Good for financial data, transactions  

**Use when:**  
Data relationships matter, strong consistency required.

---

## NoSQL Databases (Non-Relational)

Examples: MongoDB, Cassandra, DynamoDB

- Schema-less  
- Horizontally scalable  
- Great for high-volume reads/writes  
- No JOINs  

**Use when:**  
High scale, flexible schema, simple queries.

---

## Database Scaling

1. **Vertical Scaling** → stronger machine  
2. **Read Replicas** → scale read queries  
3. **Partitioning (Sharding)** → split data across DBs  
4. **Indexing** → faster queries  

---

## Consistency Models

- **Strong Consistency** → up-to-date data  
- **Eventual Consistency** → updates propagate over time  

---

## Summary

Choose SQL for consistency and relationships.  
Choose NoSQL for massive scale and simple access patterns.
