# 7. Databases

### 61. Why can’t we simply store everything in Python variables?
Variables usually exist only while a process is running and are not designed to provide durable, shared, searchable storage. A database persists data, coordinates concurrent access, and provides tools to query and protect it.

### 62. Why do applications need databases?
Applications use databases to store information beyond a single run and retrieve or update it reliably. Databases provide organization, query capabilities, concurrency control, and recovery features.

### 63. What happens when you click “Save”?
The application sends the new or changed data to its server, which validates it and issues a database operation. The database commits the change to its storage according to its durability settings, and the application reports success or an error.

### 64. Where does the data physically go?
The database writes data to persistent storage managed by the server or database service, often using files on SSDs and additional logs or replicas. The exact location depends on the deployment and provider; a cloud database still uses physical machines in data centers.

### 65. What is a table?
A table is a named structure in a relational database that organizes records into rows and defined columns.

### 66. What is a row?
A row is one record in a table, containing values for that record's columns.

### 67. What is a column?
A column is a named attribute in a table, usually with a defined data type and constraints.

### 68. Why do we need primary keys?
A primary key uniquely identifies each row so it can be referenced and updated reliably. It also helps enforce that records are distinct.