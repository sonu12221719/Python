### **1. Exception Handling**

**1. What is exception handling in Python?**
Exception handling is a mechanism to deal with runtime errors so that the normal flow of the program is not interrupted.

**2. What is the difference between syntax errors and runtime errors?**
Syntax errors occur due to incorrect code structure before execution, while runtime errors occur during execution due to invalid operations.

**3. How do you handle exceptions using `try`, `except`?**
You handle exceptions by placing risky code inside a `try` block and writing error-handling code inside an `except` block.

```python
try:
    x = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero")
```

**4. What is the difference between `except Exception` and specific exceptions?**
`except Exception` catches all exceptions derived from the `Exception` class, while specific exceptions catch only particular error types.

**5. What is the use of `finally` in exception handling?**
The `finally` block is used to execute code regardless of whether an exception occurs or not.

---

### **2. File Handling**

**6. How do you open a file in Python?**
You open a file using the `open(filename, mode)` function.

**7. What is the difference between text mode (`'t'`) and binary mode (`'b'`)?**
Text mode reads/writes data as text, while binary mode reads/writes raw bytes.

**8. What is the difference between `read()`, `readline()`, and `readlines()`?**

* `read()` reads the whole file at once.
* `readline()` reads one line at a time.
* `readlines()` reads all lines into a list.

**9. What is the difference between `w`, `a`, and `x` modes when opening a file?**

* `'w'` overwrites the file if it exists.
* `'a'` appends data to the file.
* `'x'` creates a new file but raises an error if it already exists.

**10. What is the use of the `with open()` statement in file handling?**
It is used for automatic file handling because it closes the file automatically after use.

---

### **3. Object-Oriented Programming (OOP) Basics**

**11. What is a class in Python?**
A class is a blueprint for creating objects with attributes and methods.

**12. What is an object in Python?**
An object is an instance of a class that represents a specific entity with properties and behavior.

**13. What is the difference between a class variable and an instance variable?**
A class variable is shared across all instances, while an instance variable belongs only to a particular object.

**14. What is the use of `__init__` method in a class?**
It is a constructor used to initialize instance variables when an object is created.

**15. What is the difference between `self` and `cls`?**
`self` refers to the current instance of the class, while `cls` refers to the class itself.

---

### **4. OOP Concepts**

**16. What is inheritance in Python?**
Inheritance allows a class to derive properties and methods from another class.

**17. What are the different types of inheritance supported in Python?**
Python supports single, multiple, multilevel, hierarchical, and hybrid inheritance.

**18. What is method overriding in Python?**
It occurs when a child class defines a method with the same name as the parent class, replacing its behavior.

**19. What is the difference between abstraction and encapsulation?**

* Abstraction hides implementation details and shows only essential features.
* Encapsulation bundles attributes and methods while restricting direct data access.

**20. What is the use of `super()` function in Python?**
It is used to call methods of a parent class from within a child class.

---

### **5. Modules and Libraries**

**21. What is the difference between a Python module and a package?**
A module is a single Python file, while a package is a collection of modules in a directory with an `__init__.py` file.

**22. What is the use of `__name__ == "__main__"` in Python?**
It ensures certain code runs only when the file is executed directly, not when imported.

**23. How do you import a module in Python?**
You use the `import` statement, e.g., `import math`.

**24. What is the difference between `import module` and `from module import`?**

* `import module` imports the whole module.
* `from module import name` imports specific functions or classes.

**25. What are some commonly used built-in Python modules?**
Some common modules are `os`, `sys`, `math`, `random`, `datetime`, and `json`.

---

### **6. Miscellaneous Basics**

**26. What is Python’s garbage collection?**
It automatically frees memory by removing unused objects through reference counting and cyclic garbage collection.

**27. What is the difference between shallow copy and deep copy?**
A shallow copy copies references to nested objects, while a deep copy creates independent copies of all objects.

**28. What are Python’s built-in functions (like `len()`, `type()`, `id()`, `dir()`)?**

* `len()` → returns length
* `type()` → returns data type
* `id()` → returns memory address
* `dir()` → lists attributes and methods

**29. What is the difference between `==` and `!=` vs `is` and `is not`?**

* `==` and `!=` compare values.
* `is` and `is not` compare memory identity (whether two variables point to the same object).

**30. What are Python’s naming conventions for variables, classes, and functions?**

* Variables: lowercase\_with\_underscores
* Classes: PascalCase
* Functions: lowercase\_with\_underscores

---

