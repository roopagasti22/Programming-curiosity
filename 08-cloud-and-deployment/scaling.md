# 10. Real-World Software (continued)

### 93. What changes when 1 million users use it?
Traffic, data volume, and concurrency rise, making bottlenecks, reliability, and operating cost more important. The system may need multiple application instances, load balancing, caching, queues, database optimization, and careful capacity planning.

### 94. Why can’t we simply buy one huge computer?
A bigger machine can help, but it has cost, capacity, and failure limits and can become a single point of failure. Distributing work across machines can add capacity and resilience, at the cost of more operational and coordination complexity.

### 99. How does Netflix/YouTube/Instagram handle millions of users?
Large services combine distributed infrastructure, replication, caching and content-delivery networks, load balancing, data partitioning, and automated monitoring and recovery. Their exact designs are proprietary and evolve; no single technique alone handles every workload.

### 100. If you had to build WhatsApp from scratch, what would you need?
You would need clients, identity and contact systems, reliable message delivery, storage, push notifications, media handling, encryption and key management, moderation and abuse controls, and scalable infrastructure. You would also need operations, backups, monitoring, privacy protections, and a way to handle failures and user growth.