# Scalability

Scalability is the ability of a system to **handle increased load** (more users, traffic, or data) by adding resources while maintaining good performance.

---

## Types of Scalability

### 1. Vertical Scaling (Scale Up)
Adding more power to a single machine.  
- + Simple  
- + No code changes  
- – Hardware limit  
- – Single point of failure  

### 2. Horizontal Scaling (Scale Out)
Adding more machines and distributing load.  
- + Highly scalable  
- + Fault-tolerant  
- – More complex to implement  

---

## How Systems Scale

1. **Add Load Balancer**  
   Distributes traffic across multiple servers.

2. **Use Caching**  
   Reduce load on database and improve speed (Redis, CDN).

3. **Database Scaling**  
   - Read replicas  
   - Sharding (split data across servers)  
   - Indexing  

4. **Make Services Stateless**  
   Store sessions in DB/Redis so servers can scale easily.

5. **Async Processing**  
   Use queues for heavy tasks (email, video processing).

---

## Signs of Good Scalability (Interview Points)

- Horizontal scaling with stateless servers  
- Load balancer in front of services  
- Caching at multiple layers  
- DB read replicas + sharding  
- CDN for static content  
- Message queues for background work  

---

## Summary

Scalability = handling more load with predictable performance.  
Start simple → scale using load balancing, caching, DB optimization, and horizontal scaling.
