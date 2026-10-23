# 10. Real-World Software

### 91. Where does your application actually run after deployment?
Its code runs on machines provided by a hosting platform, cloud provider, data center, or the user's own device. A deployed application may be split among browsers, application servers, databases, and other services in multiple locations.

### 92. What happens when 1 user uses your application?
The user's device runs the interface and sends requests to the application service. The service processes each request, may read or write a database, and sends a response back; logs and monitoring can record how the request went.

### 95. What is a server?
A server is a computer or program that provides services to clients over a network. It listens for requests, performs work, and returns responses; the word can refer to the software role, the physical machine, or both.

### 98. What happens when a server crashes?
Requests to that instance fail until it restarts or another instance handles them. Monitoring and health checks can detect the failure, while load balancers, replicas, and recovery procedures help restore service; unsaved in-memory state may be lost.