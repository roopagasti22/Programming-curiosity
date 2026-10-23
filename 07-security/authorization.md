# 8. Security Curiosity (continued)

### 76. What happens if someone changes an API request?
The server must treat every request as untrusted: validate its fields, authenticate the caller, and authorize the requested action against server-side rules. TLS helps prevent in-transit tampering, but it cannot stop a user from editing a request they control.

### 77. What is CORS?
Cross-Origin Resource Sharing is a browser-enforced mechanism that uses server response headers to decide whether a web page from one origin may read a response from another. It is not authentication or a general server-side access-control system.

### 78. How does a server know whether you are authorized?
The server identifies the caller from a validated session or credential, then checks permissions and policies for the specific resource and action. These checks must happen on the server for every protected operation.

### 80. How can one careless line of code expose millions of users?
A small mistake—such as skipping an authorization check, logging secrets, or building an unsafe query—can affect every request using that code path. Automated tests, least privilege, code review, monitoring, and careful handling of sensitive data help reduce the impact.