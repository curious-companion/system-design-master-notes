# Message Queues

Message Queues (MQ) enable **asynchronous processing** by decoupling components.

Examples: Kafka, RabbitMQ, AWS SQS, Google Pub/Sub

---

## Why Use Queues?

- Smooth out traffic spikes  
- Offload heavy tasks  
- Increase reliability  
- Decouple services  

---

## How It Works

1. Producer sends message → Queue  
2. Consumer reads message → Processes it  

Example:  
User uploads video → Queue → Background worker encodes video.

---

## When to Use Queues

- Sending emails  
- Push notifications  
- Video/image processing  
- Payment processing  
- Log pipelines  

---

## Key Concepts

- **Producer** – sends messages  
- **Consumer** – processes messages  
- **At-Least-Once Delivery** (most common)  
- **Idempotency** – handle duplicate messages safely  

---

## Benefits in System Design

- Improves throughput  
- Reduces latency  
- Allows scaling consumers separately  
- Prevents overload during spikes  
