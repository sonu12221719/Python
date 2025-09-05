
## **1. Advanced OOP & Classes**

**Q1. What are abstract base classes in Python?**
They are classes from the `abc` module that define abstract methods which must be implemented by subclasses, enforcing an interface.

**Q2. How do you achieve polymorphism in Python?**
By defining the same method name in different classes, allowing objects to be used interchangeably (e.g., `len()` works on lists, strings, dicts).

**Q3. What are mixins in Python OOP?**
Small, reusable classes that provide additional functionality when combined with other classes via multiple inheritance.

**Q4. What is multiple inheritance and what problem can it cause (MRO)?**
It means inheriting from multiple parent classes. It can cause method resolution conflicts, handled by Python’s **Method Resolution Order (MRO)**.

**Q5. What is the diamond problem in inheritance? How does Python handle it?**
When a class inherits from two classes that share a common ancestor, leading to ambiguity. Python resolves this using **C3 linearization (MRO)**.

---

## **2. Advanced Functions & Decorators**

**Q6. What are higher-order functions in Python?**
Functions that take other functions as arguments or return functions (e.g., `map`, `filter`).

**Q7. What is the difference between a decorator and a context manager?**

* Decorator: modifies a function’s behavior at call time.
* Context manager: manages resources for a code block using `with`.

**Q8. How do you create a custom context manager using `__enter__` and `__exit__`?**
By defining a class with `__enter__` (setup) and `__exit__` (teardown).

**Q9. What is `functools.lru_cache` and when would you use it?**
A decorator that caches function results for given inputs to speed up repeated calls. Useful in expensive or recursive computations.

**Q10. What is the difference between `staticmethod`, `classmethod`, and normal methods?**

* Normal method: takes `self`, works on instance.
* Classmethod: takes `cls`, works on class state.
* Staticmethod: no `self`/`cls`, like a regular function inside a class.

---

## **3. Iterators, Generators & Async**

**Q11. What is the difference between a generator function and a generator expression?**

* Generator function: defined with `def` and `yield`.
* Generator expression: compact form like list comprehension but with `()`.

**Q12. How do `yield` and `yield from` differ?**

* `yield`: yields single values.
* `yield from`: delegates to another generator/iterator.

**Q13. What are coroutines in Python?**
Special functions declared with `async def` that can be paused/resumed with `await`.

**Q14. What is the difference between `async` and `await`?**

* `async`: defines a coroutine.
* `await`: pauses coroutine execution until result is available.

**Q15. What is the difference between multiprocessing and multithreading in Python?**

* Multithreading: multiple threads share same memory, limited by GIL.
* Multiprocessing: runs separate processes with independent memory, bypassing GIL.

---

## **4. Memory Management & Performance**

**Q16. What is Python’s memory model?**
Python uses private heap memory managed by the interpreter; memory allocation and garbage collection are automatic.

**Q17. What are memory views in Python?**
Objects that allow direct access to an array or buffer’s memory without copying, efficient for large data.

**Q18. How does Python’s garbage collector work with reference cycles?**
Uses reference counting plus a cyclic garbage collector to detect and clean up cycles.

**Q19. What is the difference between shallow copy, deep copy, and deepcopy with weak references?**

* Shallow copy: copies outer object, references inner objects.
* Deep copy: recursively copies everything.
* Weak references: don’t increase reference count, allowing GC cleanup.

**Q20. What is the difference between Python’s list and array module?**

* List: general-purpose, heterogeneous, dynamic.
* `array`: fixed-type, more memory-efficient for numerical data.

---

## **5. Advanced Modules & Tools**

**Q21. What is the difference between `__new__` and `__init__` in Python?**

* `__new__`: creates the object (constructor).
* `__init__`: initializes the object’s attributes.

**Q22. What is the difference between `repr()` and `str()` methods?**

* `repr()`: unambiguous representation (for developers).
* `str()`: readable representation (for users).

**Q23. What are Python descriptors?**
Objects that define custom behavior for attribute access using `__get__`, `__set__`, `__delete__`.

**Q24. What is monkey patching in Python?**
Dynamically modifying or replacing methods/attributes of a class or module at runtime.

**Q25. What is metaclass in Python?**
A class of a class that controls how classes are created and behaves, by customizing `__new__` or `__init__`.

---

## **6. Concurrency & Internals**

**Q26. What is the Global Interpreter Lock (GIL) and why does it exist?**
A mutex that allows only one thread to execute Python bytecode at a time, ensuring memory safety.

**Q27. How can you bypass the GIL in Python?**
By using multiprocessing, C extensions, or releasing the GIL in native code.

**Q28. What is the difference between synchronous and asynchronous programming in Python?**

* Synchronous: tasks execute one after another.
* Asynchronous: tasks can pause and resume, enabling concurrency.

**Q29. What is the difference between CPU-bound and I/O-bound tasks in Python?**

* CPU-bound: heavy computation, best with multiprocessing.
* I/O-bound: waiting for I/O (network, file), best with async or threading.

**Q30. What is `multiprocessing.Queue` and how is it different from `queue.Queue`?**

* `multiprocessing.Queue`: used for process-safe communication, works across processes.
* `queue.Queue`: thread-safe queue, used for threads in same process.

---

