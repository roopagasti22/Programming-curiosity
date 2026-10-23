# 2. Your First Line of Code

### 11. What happens internally when you write `x = 10`?
The language evaluates `10` and binds the name `x` to that value (in Python, to an integer object). The exact representation and storage are implementation details, not a promise that a named box is created.

### 12. Where is 10 stored?
While the program runs, the integer's representation is held in memory managed by the runtime and operating system. Its physical location can change and usually is not something a programmer needs to know.

### 13. Where is x stored?
In Python, a name such as `x` is an entry in a namespace that refers to an object. Depending on context, the namespace may be associated with a module, function, or object; it is not necessarily a fixed memory slot.

### 14. Is x actually the value 10?
Not exactly: `x` is a name bound to the integer value `10` (represented by an object in Python). This distinction matters when multiple names refer to the same mutable object.

### 15. What happens when you write `x = 10` and then `x = 20`?
The name `x` is rebound to `20`; the second assignment does not edit the integer `10`. Other names that still refer to `10` remain bound to it.

### 16. What happens to 10?
If nothing else refers to the old value, it becomes eligible for reclamation. Python implementations may reuse or retain memory, so becoming unused does not mean the memory is immediately returned to the operating system.

### 17. What happens when you write `a = b = c = 100`?
Python evaluates the right-hand expression and binds each name to that result. It does not mean that three independent copies must be made.

### 18. Are a, b and c three copies of 100?
For this immutable integer, the names refer to the same resulting value; whether the implementation reuses an internal object is an optimization detail. With a mutable object, chained assignment makes all names refer to the same object, so a change through one name can be seen through the others.