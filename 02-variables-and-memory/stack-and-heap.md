# 2. Your First Line of Code (continued)

### 19. What happens to variables when a function finishes?
When a function returns, its local namespace and call state are no longer active. Objects referenced only by those locals may become reclaimable, but objects also referenced elsewhere remain available; exact memory cleanup timing depends on the runtime.

# 3. Memory — The Hidden World

### 26. What is a stack?
A call stack tracks active function calls, including return locations and local execution state. Each call adds a frame and returning removes that frame; languages and runtimes may store some local data differently.

### 27. What is a heap?
The heap is a broad term for memory used for dynamically managed objects whose lifetimes are not simply tied to one function call. A runtime tracks allocations there, but the exact layout varies by language and implementation.