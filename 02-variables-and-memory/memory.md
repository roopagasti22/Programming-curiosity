# 3. Memory — The Hidden World

### 21. What is RAM actually doing while your program runs?
RAM holds the program's active instructions and data so the processor can access them quickly. The operating system manages which memory belongs to each process and may move inactive pages between RAM and storage.

### 22. What is the difference between RAM and storage?
RAM is fast working memory and is normally cleared when power is lost; storage such as an SSD retains files without power. Programs are loaded from storage into memory to run.

### 23. Where does a Python variable live?
A Python name lives in a namespace, and it refers to an object managed by the Python runtime. The object and name mapping occupy process memory, but their exact locations are implementation-dependent.

### 24. What is a memory address?
A memory address identifies a location in a process's virtual address space. The operating system maps virtual addresses to physical memory, so an address a program sees is not necessarily a direct physical RAM location.

### 25. Why can’t we normally see memory addresses in Python?
Python hides addresses to provide a simpler, safer object model that works across implementations and platforms. Some diagnostic tools can expose identity or low-level details, but those should not be treated as stable addresses.