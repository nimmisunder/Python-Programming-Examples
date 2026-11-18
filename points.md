What is the difference between Python Arrays and lists?

Arrays in python can only contain elements of same data types i.e., data type of array should be homogeneous. It is a thin wrapper around C language arrays and consumes far less memory than lists.
Lists in python can contain elements of different data types i.e., data type of lists can be heterogeneous. It has the disadvantage of consuming large memory.
pass does nothing, continue skips an iteration, and break exits a loop
1. Variables and data types
- Python is dynamically typed.
- type() checks the data type.
- int, float, complex, str, bool are built-in types.
- None represents the absence of a value.
2. List, Tuple, Set and Dictionary
- List → Ordered, mutable, allows duplicates.
- Tuple → Ordered, immutable, allows duplicates.
- Set → Unique elements, no guaranteed order.
- Dictionary → Key-value pairs; keys must be unique.
3. Loops
- for → Iterates over a sequence or iterable.
- while → Repeats while a condition is true.
- break → Exits the loop.
- continue → Skips the current iteration.
- pass → Does nothing; placeholder statement.
4. Functions
- def → Defines a function.
- return → Sends a result back to the caller.
- print() → Displays output.
- *args → Accepts variable positional arguments.
- **kwargs → Accepts variable keyword arguments.
- Lambda → Small anonymous function.
5. String methods
- upper() → Uppercase.
- lower() → Lowercase.
- strip() → Removes leading and trailing whitespace.
- split() → String to list.
- join() → List of strings to string.
- replace() → Replaces text.
- [::-1] → Reverses a string.
- Strings are immutable.
6. Scope
- Local → Inside a function.
- Enclosing → Inside an outer function.
- Global → Outside functions.
- Built-in → Python-provided names.
- global → Modifies a global variable.
- nonlocal → Modifies an enclosing variable.
- LEGB → Local, Enclosing, Global, Built-in.
7. Advanced Python
- Decorator → Extends function behaviour.
- Generator → Uses yield to produce values lazily.
- async → Defines a coroutine.
- await → Suspends a coroutine while awaiting an operation.
- GIL → In traditional GIL-enabled CPython, only one thread executes Python bytecode at a time.
- Multithreading → Useful for I/O-bound tasks.
- Multiprocessing → Useful for CPU-bound tasks.
- Reference counting → Tracks references to objects.
8. Memory management
- Python manages memory automatically.
- Reference counting tracks object references.
- Garbage collection handles reference cycles.
- del removes a reference, not necessarily the object itself.
- Mutable objects can be modified.
- Immutable objects cannot be modified in place.
9. Coding interview patterns
- List comprehension → Concise list creation.
- set() → Removes duplicates.
- sorted() → Returns a new sorted list.
- .sort() → Sorts a list in place.
- enumerate() → Gives index and element.
- zip() → Combines iterables.
- Sliding window → Useful for substring and subarray problems.
