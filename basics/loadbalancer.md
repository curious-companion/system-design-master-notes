# Load Balancer

A Load Balancer distributes incoming traffic across multiple servers so that no single machine becomes overloaded.  
It improves **scalability**, **performance**, and **fault tolerance**.

---

## Why Load Balancing?

- Prevents server overload  
- Increases system availability  
- Enables horizontal scaling  
- Provides automatic failover  
- Smooths traffic spikes  

---

## How It Works

Client → **Load Balancer** → Multiple Backend Servers  
The LB decides *which server* should handle each request.

---

## Types of Load Balancing

### 1. **Layer 4 (Transport Level)**
- Uses IP + Port  
- Fast, lightweight  
- Limited routing logic  

### 2. **Layer 7 (Application Level)**
- Routes based on URL, headers, cookies  
- Smart routing (e.g., `/api` vs `/static`)  
- Used by Nginx, HAProxy, Envoy  

---

## Common Load Balancing Algorithms

- **Round Robin** — each server gets request in turns  
- **Weighted Round Robin** — powerful server gets more traffic  
- **Least Connections** — server with fewest active connections  
- **IP Hash** — same client goes to same server  
- **Random** — simple, sometimes effective  

---

## Health Checks

Load balancer continuously checks if a server is:
- Alive  
- Responding fast  
- Returning correct responses  

If not, it removes the server from rotation (failover).

---

## Sticky Sessions (Session Affinity)

Sometimes the same user must hit the same server:
- Shopping carts  
- Login sessions  

Approaches:
- IP-based routing  
- Cookies  
- Use Redis/session store to avoid stickiness  

---

## Load Balancer in System Design

You mention LB when:
- You scale your app horizontally  
- You want high availability  
- You want to handle millions of requests  
- You’re building distributed systems  

---

## Summary

Load Balancer = **traffic distributor** for scalable, reliable systems.  
Used with:
- Multiple app servers  
- Caching  
- Replication  
- Auto-scaling groups  

It’s one of the first components added when scaling any system.
