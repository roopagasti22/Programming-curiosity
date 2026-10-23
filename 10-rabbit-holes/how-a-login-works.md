# 🔥 Rabbit Hole Questions

### Rabbit Hole 4. When I click Login, how does my password travel from my phone to the server and come back as “Login successful”?
The app sends the credentials over HTTPS, which protects them in transit with TLS. The server looks up the account and compares a password hash computed with the stored salt and password-hashing settings; it should never store the plain password. On success, it creates a session or token, and the app receives a response. Later requests include the session proof, which the server validates.

### Rabbit Hole 7. What happens if two users try to modify the same database record at exactly the same time?
The database coordinates concurrent writes using locks, version checks, or another concurrency-control strategy. Depending on isolation and application logic, one update may wait, fail with a conflict, or overwrite another; applications should detect and handle conflicts and use transactions for related changes. See [transactions.md](../06-databases/transactions.md) for the database concepts behind this.