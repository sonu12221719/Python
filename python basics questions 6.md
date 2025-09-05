## 🔹 **1. Advanced Concurrency & Async**

**1. What is the difference between threads and asyncio in Python?**
Threads use OS-level context switching to achieve concurrency, while `asyncio` is cooperative multitasking based on an event loop, where tasks yield control explicitly (`await`) instead of preemption.

**2. How does Python’s `asyncio` event loop work?**
The event loop schedules and runs asynchronous tasks (coroutines), switching between them when they hit `await` points, allowing I/O-bound operations to run efficiently without blocking.

**3. What is the difference between `asyncio.create_task()` and `await`?**
`await` runs a coroutine and waits for its result, while `asyncio.create_task()` schedules the coroutine to run in the background and returns a task object that can be awaited later.

**4. What is an `async generator`?**
An async generator is defined with `async def` and `yield`, allowing asynchronous iteration using `async for`, useful for streaming data over time.

**5. What are Python Futures and Promises?**
A `Future` represents a placeholder for a result that will be available in the future. In Python, they are used in `concurrent.futures` and `asyncio`. A promise is the conceptual abstraction that resolves into a future result.

---

## 🔹 **2. Networking & Sockets**

**6. How do you create a simple TCP server in Python using `socket`?**
By creating a socket with `socket.AF_INET` and `socket.SOCK_STREAM`, binding it to an address, listening with `.listen()`, and accepting connections with `.accept()`.

**7. What is the difference between TCP and UDP sockets in Python?**
TCP (`SOCK_STREAM`) is connection-oriented, reliable, and ordered, while UDP (`SOCK_DGRAM`) is connectionless, faster, but does not guarantee delivery or order.

**8. What is the use of the `select` module in networking?**
It monitors multiple sockets for readiness (read, write, or error states), allowing efficient I/O multiplexing without blocking on a single socket.

**9. How do you implement a simple HTTP server in Python?**
You can use the built-in `http.server` module with `python -m http.server`, or subclass `BaseHTTPRequestHandler` for custom behavior.

**10. What is the difference between `requests` and `http.client` libraries?**
`requests` is a high-level HTTP library for making web requests easily, while `http.client` is a low-level library that provides raw HTTP protocol handling.

---

## 🔹 **3. Advanced Modules & Standard Library**

**11. What is the difference between `deepcopy` in `copy` module and `pickle`?**
`deepcopy` creates a new in-memory copy of objects, while `pickle` serializes objects into a byte stream that can be saved to disk or sent over a network.

**12. How does Python’s `subprocess` module work?**
It allows you to spawn new processes, connect to their input/output/error pipes, and obtain their return codes, providing better control than `os.system`.

**13. What is the use of the `contextlib` module?**
It provides utilities for creating and working with context managers, such as `contextmanager` decorator, `ExitStack`, and suppressing exceptions.

**14. What is the `dataclasses` module introduced in Python 3.7?**
It automatically generates boilerplate methods (`__init__`, `__repr__`, `__eq__`, etc.) for classes, reducing repetitive code when defining data containers.

**15. What is the difference between `logging` and `print()` for debugging?**
`print()` outputs simple messages, while `logging` provides configurable log levels, timestamps, output destinations (file, console, etc.), and better control in production.

---

## 🔹 **4. Memory & Optimization**

**16. How do you profile memory usage in Python?**
Using tools like `tracemalloc`, `memory_profiler`, or external profilers (e.g., `guppy3`) to track memory allocation and leaks.

**17. What are Python’s weak references (`weakref` module)?**
They allow referencing objects without preventing garbage collection, useful for caching where you don’t want references to keep objects alive unnecessarily.

**18. What is interning of strings in Python?**
Interning is the practice of storing only one copy of immutable strings with the same value, which optimizes memory and comparisons for common strings.

**19. How does Python manage immutable vs mutable objects in memory?**
Immutable objects (like tuples, strings) cannot change, so Python reuses them where possible, while mutable objects (like lists, dicts) are stored uniquely and can be modified.

**20. What is the difference between `sys.getsizeof()` and `__sizeof__()`?**
`__sizeof__()` returns only the memory consumed by the object itself, while `sys.getsizeof()` includes additional garbage collector overhead.

---

## 🔹 **5. Advanced Internals**

**21. What is the Python C API?**
It’s an interface that allows C code to interact with Python objects, enabling extensions, embedding Python in C applications, and improving performance.

**22. How does Python’s bytecode execution work internally?**
Python source is compiled into bytecode (`.pyc`), which is executed by the Python Virtual Machine (PVM), an interpreter loop that dispatches bytecode instructions.

**23. What is the difference between CPython, PyPy, and Jython?**

* **CPython**: Default C-based implementation.
* **PyPy**: Python implementation with a JIT compiler for speed.
* **Jython**: Python implemented on top of the JVM, interoperable with Java.

**24. What are Python’s code objects?**
Code objects represent compiled Python bytecode, containing metadata like constants, variable names, and line numbers, created when functions or modules are compiled.

**25. What is the difference between a compiled `.pyc` file and a `.py` file?**
A `.py` file contains human-readable source code, while a `.pyc` file contains bytecode that Python can load directly, speeding up startup.

---

## 🔹 **6. Performance Tuning & Best Practices**

**26. How do you use `cProfile` to analyze Python code performance?**
Run `python -m cProfile script.py`, which measures execution time per function call, helping identify bottlenecks.

**27. What is memoization and how can you implement it in Python?**
Memoization is caching results of expensive function calls to reuse them later. It can be implemented manually with a dictionary or using `functools.lru_cache`.

**28. What is the difference between a normal dictionary and `collections.OrderedDict`?**
In Python 3.7+, regular dicts preserve insertion order, but `OrderedDict` also provides methods like `move_to_end()` and equality checks based on order.

**29. How can you improve performance using `multiprocessing.Pool`?**
By parallelizing CPU-bound tasks across multiple processes, each with its own interpreter, avoiding GIL limitations.

**30. What is the benefit of using Cython with Python?**
Cython translates Python code into C, which compiles into machine code, offering significant performance improvements, especially for numeric and loop-heavy operations.

---


