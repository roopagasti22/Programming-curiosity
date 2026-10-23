# 2. Your First Line of Code (continued)

### 20. Who cleans unused memory?
The language runtime or memory manager reclaims memory when objects are no longer needed; Python commonly uses reference counting plus a cyclic garbage collector. Programmers still need to release external resources such as files and connections explicitly.

# 3. Memory — The Hidden World (continued)

### 28. What is garbage collection?
Garbage collection is automatic detection and reclamation of memory occupied by objects a program can no longer reach. It reduces the need for manual deallocation but does not manage every resource automatically.

### 29. Why doesn’t unused memory remain forever?
Runtimes reuse memory from objects that are no longer reachable, so long-running programs can continue allocating. They may keep reclaimed memory for reuse rather than immediately returning it to the operating system.

### 30. What happens when your program consumes too much memory?
Allocation may fail, the runtime may raise an out-of-memory error, or the operating system may terminate the process. Excessive memory use can also trigger slow paging; reducing retained data or processing in smaller batches can help.