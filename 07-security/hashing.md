# 8. Security Curiosity (continued)

### 72. Where is your password stored?
A well-designed service stores a salted password hash, not the original password, in a protected credential store or database. The hash is computed with a password-specific function such as Argon2id, scrypt, or bcrypt, configured to make guessing costly.

### 73. Why shouldn’t passwords be stored as plain text?
If a database is exposed, plain-text passwords immediately reveal users' credentials and may enable account takeovers elsewhere. A salted, deliberately slow password hash limits the usefulness of stolen records and makes each guess more expensive.

### 75. What is hashing?
Hashing maps input data to a fixed-length digest. Cryptographic hashes are designed to make it computationally infeasible to recover the input or find collisions, but password storage needs specialized slow hashing rather than a fast general-purpose hash.