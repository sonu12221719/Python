# **1. Iterators & Generators**

**91. What is an iterator in Python?**
An iterator is an object that allows sequential traversal of elements using `__iter__()` and `__next__()` methods.

**92. How do you create an iterator manually?**
By defining a class with `__iter__()` returning `self` and `__next__()` to yield elements until `StopIteration` is raised.

**93. What is the difference between iterable and iterator?**

* Iterable: Any object that can return an iterator (e.g., list, tuple, string).
* Iterator: Object that produces one element at a time using `__next__()`.

**94. What is a generator in Python?**
A generator is a function that uses `yield` to produce a sequence of values lazily (one at a time).

**95. What is the difference between `return` and `yield`?**

* `return` ends the function and returns a value.
* `yield` pauses the function, saving its state, and resumes from there on the next call.

---

### **2. Decorators**

**96. What is a decorator in Python?**
A decorator is a function that takes another function as input, extends or modifies its behavior, and returns a new function.

**97. What are some common use cases of decorators?**
Logging, authentication, caching, measuring execution time, and access control.

**98. What is the difference between `@staticmethod` and `@classmethod`?**

* `@staticmethod`: Method that doesn’t access class/instance.
* `@classmethod`: Method that takes `cls` as first parameter and can modify class-level state.

**99. What is the use of `@property` decorator?**
It is used to make a method behave like an attribute (getter), allowing controlled access to private variables.

**100. Can decorators be chained?**
Yes, multiple decorators can be applied to a single function by stacking them.

---

### **3. Virtual Environments & pip**

**101. What is a Python virtual environment?**
A self-contained directory that isolates dependencies for a Python project.

**102. How do you create a virtual environment?**
Using:

```bash
python -m venv env
```

**103. How do you activate a virtual environment?**

* Windows: `env\Scripts\activate`
* Linux/Mac: `source env/bin/activate`

**104. What is pip in Python?**
`pip` is Python’s package installer used to install and manage external libraries.

**105. How do you list installed packages in pip?**
By running:

```bash
pip list
```

---

### **4. Unit Testing Basics**

**106. What is unit testing in Python?**
Unit testing is testing individual units (functions, methods, classes) to ensure they work as expected.

**107. Which built-in module is used for testing in Python?**
The `unittest` module.

**108. How do you write a simple unit test?**
By creating a class inheriting from `unittest.TestCase` and writing methods starting with `test_`.

**109. What is the difference between `assertEqual` and `assertTrue`?**

* `assertEqual(a, b)` checks if `a == b`.
* `assertTrue(x)` checks if `x` is `True`.

**110. What is test-driven development (TDD)?**
A software approach where tests are written before the actual code implementation.

---

### **5. Python Utilities**

**111. What is the use of the `os` module?**
It allows interaction with the operating system (file system, environment variables, processes).

**112. What is the use of the `sys` module?**
It provides system-specific functions and access to Python runtime environment (e.g., `sys.argv`, `sys.exit`).

**113. How do you get the current date and time in Python?**
Using the `datetime` module:

```python
from datetime import datetime
print(datetime.now())
```

**114. What is the difference between `time.sleep()` and `datetime`?**

* `time.sleep()` pauses execution.
* `datetime` works with dates and times.

**115. What is the use of the `logging` module?**
It is used to record logs (info, warning, error) instead of printing, useful for debugging and monitoring.

---

### **6. Best Practices & Miscellaneous**

**116. What are Python’s naming conventions for constants?**
Constants are usually written in all uppercase letters with underscores (e.g., `MAX_SIZE = 100`).

**117. What is PEP 8 in Python?**
PEP 8 is Python’s official style guide for writing clean and readable code.

**118. What is the difference between `is` and `==`?**

* `is`: Checks object identity (same memory reference).
* `==`: Checks value equality.

**119. How do you install external libraries in Python?**
Using:

```bash
pip install package_name
```

**120. What are Python virtualenv and venv differences?**

* `venv`: Built-in lightweight environment manager (Python 3.3+).
* `virtualenv`: Third-party tool, older but more feature-rich, works for multiple Python versions.

---


