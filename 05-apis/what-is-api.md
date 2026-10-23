# 6. APIs — The Invisible Communication

### 51. What exactly is an API?
An Application Programming Interface is a defined way for software components to request services or exchange data. It specifies available operations, inputs, outputs, and rules without requiring callers to know the implementation.

### 52. Why can’t two applications simply access each other’s variables?
Applications usually run in separate processes or on separate machines, with isolated memory and different lifecycles. An API provides a controlled, agreed-upon boundary for communication rather than unsafe direct access to another program's internal state.

### 53. What happens when a React application calls a Node/Python API?
The browser-side application sends an HTTP request, often containing JSON, to an API endpoint. A server process validates and handles it, may access other services or a database, and returns an HTTP response that the React application can process.

### 56. Why do APIs commonly use JSON?
JSON is a compact, text-based data format supported by most programming languages and easy to inspect. It works well for common structured data, although APIs can use other formats when their needs require them.