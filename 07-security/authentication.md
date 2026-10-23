# 8. Security Curiosity

### 71. How does a website know who you are after login?
After verifying your credentials, the server creates a session or issues a token representing the authenticated user. The browser sends that proof with later requests, and the server validates it before associating a request with the account.

### 79. What is a token?
A token is a piece of data that carries claims or serves as proof in a protocol. In login systems it may represent a session or identity; it must be protected, validated, and given an appropriate lifetime because possession can grant access.