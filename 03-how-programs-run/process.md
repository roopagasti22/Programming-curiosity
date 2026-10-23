# 4. When You Run a Program

### 31. Who receives the command `python app.py`?
The command is first handled by the shell or command-line environment. It finds and starts the `python` executable, passing `app.py` as an argument; in an IDE, the IDE may launch that process on your behalf.

### 32. How does the operating system know where Python is?
The shell searches configured locations such as directories in `PATH`, or uses an explicitly supplied executable path. The operating system then loads that executable and its required libraries.

### 33. What is a process?
A process is a running program instance managed by the operating system. It has an identity and resources such as a virtual memory space, open files, and one or more threads.

### 40. What happens when the program crashes?
An unhandled error or fatal fault can stop the process; the runtime may print an error or stack trace and the operating system records an exit status. Other programs remain separate, although they may observe that this process stopped.