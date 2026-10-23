# 🔥 Rabbit Hole Questions

### Rabbit Hole 3. When I enter google.com, how does my computer find another computer somewhere in the world?
The browser asks DNS for an address, then opens a network connection to that address. Routers forward packets across networks toward the destination; TLS secures the connection, and HTTP carries the browser's request and the server's response. The destination may be a nearby edge server rather than one fixed computer.

### Rabbit Hole 5. When I upload a photo to Instagram, where does that photo actually go?
The app sends the photo over an authenticated, encrypted connection to Instagram's service. The service validates the upload, stores the image in managed media storage, and records metadata and ownership in databases; copies or optimized versions may be distributed through a content-delivery network. The exact internal design is private and can change.

### Rabbit Hole 6. How can millions of people use the same application at the same time?
The application can run on many instances behind load balancers, with caches, queues, and databases designed for concurrent workloads. Data may be replicated or partitioned, and monitoring helps teams detect bottlenecks. Scaling requires coordinating state and handling failures, not merely adding servers.