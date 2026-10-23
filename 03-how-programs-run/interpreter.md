# 4. When You Run a Program (continued)

### 35. Where does the Python interpreter run?
The Python interpreter is itself a native program running as part of the process started by the operating system. It reads and executes Python code using the process's resources.

### 36. How does Python read your `.py` file?
Python opens the file, decodes its text, parses it, and compiles it to code objects (often cached as bytecode). The interpreter then executes those code objects.

### 37. Does Python directly understand your source code?
The runtime processes Python source through parsing and compilation before execution; it does not simply pass the text to the processor. In the standard CPython implementation, execution commonly uses bytecode interpreted by the Python Virtual Machine.

### 38. What is bytecode?
Bytecode is a compact set of instructions for a language runtime rather than a processor's native instruction set. Python can compile source into bytecode and execute it inside its virtual machine.

### 39. What is the Python Virtual Machine?
The Python Virtual Machine is the runtime machinery that executes Python bytecode and implements language behavior. It is software running on the host operating system, not a separate physical computer.