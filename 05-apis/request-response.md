# 6. APIs — The Invisible Communication (continued)

### 54. What is a request?
A request is a message asking a service to perform an operation or provide information. In HTTP it typically contains a method, URL, headers, and sometimes a body.

### 55. What is a response?
A response is the service's reply to a request. An HTTP response includes a status code and headers, and may include a body with data or an explanation of an error.

### 59. What happens if an API takes 10 seconds to respond?
The client waits until its timeout or the server responds; the user may see a loading state or timeout error. Well-designed clients set reasonable timeouts, report failures, and retry only when safe, while services monitor latency and investigate bottlenecks.

### 60. What happens if the API server is completely down?
The request cannot be completed and may fail with a connection error or gateway error. The client should explain the problem and avoid pretending the operation succeeded; redundant instances, health checks, and recovery procedures can reduce downtime.