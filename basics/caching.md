# Caching

Caching stores frequently accessed data in a faster storage layer (RAM or CDN) to reduce latency and reduce load on the database.

---

## Why Use Caching?

- Faster response times  
- Reduce DB queries  
- Handle higher traffic  
- Lower cost per request  

---

## Common Cache Layers

1. **Application Cache (in-memory)**
   - Fastest
   - Limited to one instance

2. **Distributed Cache (Redis / Memcached)**
   - Shared across servers
   - Works with horizontal scaling

3. **CDN Cache**
   - For images, videos, static content
   - Cached close to the user

---

## Cache Strategies

- **Read-Through** → App reads from cache first, falls back to DB  
- **Write-Through** → Writes to DB + cache together  
- **Write-Back** → Write to cache first, DB later  
- **Cache Aside** (Lazy Loading) → Load into cache only when needed  

---

## Eviction Policies

- **LRU** (Most common)  
- **LFU**  
- **FIFO**  

---

## When to Mention Caching in Interviews?

Whenever:
- System is read-heavy  
- DB is bottleneck  
- Speed is important  

Caching is one of the simplest ways to scale a system.
