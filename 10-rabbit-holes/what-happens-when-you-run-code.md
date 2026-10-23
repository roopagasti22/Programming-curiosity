# 🔥 Rabbit Hole Questions

### Rabbit Hole 1. When I type `x = 10`, where exactly does 10 go?
The Python runtime creates or reuses an integer object and binds the name `x` to it in the current namespace. That object and the namespace occupy the process's virtual memory, which the operating system maps onto physical memory as needed. Follow the chain: variable name → object → process memory → RAM/virtual memory → operating system. There is no single permanent physical address promised by Python.

### Rabbit Hole 2. When I type `python app.py`, what happens between pressing Enter and seeing the output?
The shell locates Python and starts a process with `app.py` as an argument. The operating system loads the interpreter; Python reads and compiles the source to code objects, executes them in its runtime, and writes output to the terminal. The operating system schedules the process and routes its input and output.

### Rabbit Hole 8. How does a program know that another program has crashed?
Programs do not automatically know. The operating system can report process exit or a failed connection; services can also use health checks, heartbeats, and timeouts to detect that a peer is no longer responding. Detection is imperfect—a slow process can look like a failed one—so systems often retry carefully or switch to a healthy instance.

### Rabbit Hole 9. If Python, JavaScript and Java are completely different languages, how can they communicate with each other?
They communicate across boundaries using shared contracts: HTTP with JSON, message queues, files, databases, or language-neutral protocols. A program can also call another language's native library through a foreign-function interface. The languages need not share internal variables; they agree on how data and operations are represented.

### Rabbit Hole 10. If the Internet disappeared tomorrow, which parts of your application would still work?
Features that run locally and need only data already stored on the device may continue to work, such as offline notes or cached pages. Login checks, remote APIs, synchronization, and cloud-hosted data would be unavailable until connectivity returned. Offline behavior must be designed explicitly, including how later changes are synchronized.