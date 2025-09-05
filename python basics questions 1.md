# Python

### **1. Basics of Python**

1. What is Python? What are its key features?
	- Python is a versatile, high-level programming language known for its simplicity, readability, and extensive capabilities. It supports multiple programming paradigms, including object-oriented, procedural, and functional programming, making it a popular choice for developers across various domains.
	- **Key Features**
		- Python is **easy to learn and use**, with a syntax that resembles plain English, making it beginner-friendly. 
		- It is an **interpreted language**, meaning code is executed line by line, which simplifies debugging. 
		- Python is **dynamically typed**, so variable types are determined at runtime, enhancing flexibility.
		- It is **cross-platform**, allowing code to run seamlessly on Windows, macOS, and Linux. 
		- Python's **extensive standard library** provides modules for tasks like file I/O, networking, and regular expressions, reducing the need for additional code. 
		- It also supports **GUI programming** through libraries like Tkinter, PyQt, and wxPython.
		- Python is **free and open-source**, enabling developers to use, modify, and distribute it without restrictions. 
		- Its **portability** ensures that code written on one platform can run on others without modification. 
		- Additionally, Python's **large community support** offers extensive resources for troubleshooting and learning.
		
2. What are Python’s advantages and disadvantages?
	
	Advantages of Python
	- ***Easy to Read, Learn, and Code:*** Python's syntax is simple and resembles English, making it beginner-friendly. This simplicity also reduces maintenance costs.
	- ***Dynamic Typing:*** Variables in Python do not require explicit declaration, allowing for dynamic coding.
	- ***Free and Open Source:*** Python is free to use and distribute, and its source code is available for modification.
	- ***Portability:*** Python code can run on various operating systems without modification, thanks to its platform-independent nature.
	- ***Extensive Libraries:*** Python boasts a wide range of libraries like NumPy, Pandas, and Django, which simplify coding and enhance functionality.
	- ***Wide Range of Applications:*** Python is used in web development, desktop GUIs, app development, artificial intelligence, data science, and more.
	- ***Extensible and Integrable:*** Python can extend to other languages like C and C++, and integrate with Java, enhancing cross-platform development.
	- ***Interpreted Language:*** Python executes code line by line, making debugging easier.
	- ***Functional, Object-Oriented, and Procedural:*** Python supports multiple programming paradigms, offering flexibility in coding.
	- ***Memory Management:*** Python uses a private heap and a built-in memory manager, ensuring efficient memory management.
	- ***Improved Productivity:*** Python's concise syntax allows developers to focus more on algorithms rather than coding.
	- ***Vast Community:*** Python has a large and active community, providing continuous support and resources.

	**Disadvantages of Python**
	- ***Slow Speed and Memory Inefficiency:*** Python's interpreted nature and dynamic typing slow down execution and increase memory usage.
	- ***Weak Mobile Computation:*** Python is rarely used for mobile applications due to its high memory consumption and slower processing.
	- ***Poor Database Access:*** Python's database access layers are less robust compared to technologies like JDBC and ODBC.
	- ***Runtime Errors:*** Dynamic typing can lead to runtime errors, making it difficult to test and debug.
	- ***Global Interpreter Lock (GIL):*** Python's GIL limits the execution of threads, affecting multithreading and concurrency.
	- ***Distinct Nomenclature:*** Python's unique syntax and terminology can be challenging for developers accustomed to other languages.
	- ***Code Size:*** Python code can become unwieldy if not properly managed, especially with large projects.
	
3. What are Python’s different applications in real life?
	Python's versatility makes it suitable for a wide range of applications:
	- ***Web Development:*** Frameworks like Django and Flask simplify building dynamic websites and web applications.
	- ***Data Science and Analytics:*** Libraries such as Pandas, NumPy, and Matplotlib make Python a go-to language for data analysis and visualization.
	- ***Artificial Intelligence and Machine Learning:*** Tools like TensorFlow, Keras, and Scikit-learn enable the development of AI and ML models.
	- ***Game Development:*** Libraries like Pygame facilitate the creation of 2D and 3D games.
	- ***Automation and Scripting:*** Python is widely used for automating repetitive tasks and writing scripts for system management.
	- ***Scientific Computing:*** Libraries like SciPy and SymPy support numerical and symbolic computations.
	- ***Desktop GUI Applications:*** Python's GUI libraries allow developers to create cross-platform desktop applications.
	- ***Web Scraping:*** Tools like BeautifulSoup and Scrapy enable extracting data from websites.
	- ***Embedded Systems and IoT:*** Python is used in devices like Raspberry Pi for IoT and robotics projects.
	- ***Finance and Healthcare:*** Python is employed for financial modeling, algorithmic trading, and medical data analysis.
4. What is PEP 8, and why is it important?
	PEP 8, or Python Enhancement Proposal 8, is the official style guide for Python code. Created by Guido van Rossum (Python's creator), Barry Warsaw, and Nick Coghlan, it provides coding conventions that help make Python code more readable and consistent across the Python ecosystem.
5. What are Python identifiers and keywords?
	**Python Identifiers:**
	- Identifiers are the names given to variables, functions, classes, modules, or other objects in Python.
	- They are user-defined names that help us identify elements in a program.
	
	**Rules for Identifiers**
	- Can contain letters (a–z, A–Z), digits (0–9), and underscores _.
	- Must not start with a digit.
		✅ name1 is valid
		❌ 1name is invalid
	- Cannot use special symbols like @, $, % in names.
	- Cannot be a Python keyword (like if, for, class).
	- Python is case-sensitive, so value and Value are different identifiers.
	
	**Python Keywords**
	- Keywords are reserved words in Python that have special meaning and purpose.
	- You cannot use keywords as identifiers.
```python
False, True, None, and, as, assert, break, class, continue, def,
del, elif, else, except, finally, for, from, global, if, import,
in, is, lambda, nonlocal, not, or, pass, raise, return, try,
while, with, yield
```


---

### **2. Data Types and Variables**

6. What are Python’s built-in data types?
	In Python, **data types** tell what kind of value a variable holds.
Python comes with several **built-in data types**, grouped into categories:

	🔹 **1. Text Type**

	* **`str`** → String (sequence of Unicode characters)

	```python
		name = "Sonu"
	```
	---
	🔹 **2. Numeric Types**

	* **`int`** → Integer numbers
	* **`float`** → Decimal (floating-point numbers)
	* **`complex`** → Complex numbers with real and imaginary part

	```python
		x = 10        # int
		y = 3.14      # float
		z = 2 + 5j    # complex
	```

	---

	 🔹 **3. Sequence Types**

	* **`list`** → Ordered, mutable collection
	* **`tuple`** → Ordered, immutable collection
	* **`range`** → Sequence of numbers (used in loops)

	```python
		fruits = ["apple", "banana", "cherry"]   # list
		point = (2, 4, 6)                        # tuple
		numbers = range(5)                       # 0,1,2,3,4
	```

	---

	🔹 **4. Mapping Type**

	* **`dict`** → Key-value pairs (like a hash map)

	```python
		student = {"name": "Sonu", "age": 21}
	```

	---

	🔹 **5. Set Types**

	* **`set`** → Unordered collection of unique items
	* **`frozenset`** → Immutable set

	```python
		a = {1, 2, 3, 3}          # {1, 2, 3}
		b = frozenset([1, 2, 3])  # cannot change
	```

	---

	## 🔹 **6. Boolean Type**

	* **`bool`** → Represents `True` or `False`

	```python
		is_active = True
	```

	---

	## 🔹 **7. Binary Types**

	* **`bytes`** → Immutable sequence of bytes
	* **`bytearray`** → Mutable sequence of bytes
	* **`memoryview`** → A view object to access memory of bytes-like objects

	```python
		x = b"hello"                    # bytes
		y = bytearray([65, 66, 67])     # bytearray
		z = memoryview(bytes(5))        # memoryview
	```

	---

	✅ **Summary Table of Built-in Data Types in Python**

	| Category | Types                              |
	| -------- | ---------------------------------- |
	| Text     | `str`                              |
	| Numeric  | `int`, `float`, `complex`          |
	| Sequence | `list`, `tuple`, `range`           |
	| Mapping  | `dict`                             |
	| Set      | `set`, `frozenset`                 |
	| Boolean  | `bool`                             |
	| Binary   | `bytes`, `bytearray`, `memoryview` |

	---


7. What is the difference between mutable and immutable data types?
		

	🔹 **1. Mutable Data Types**

	* **Definition**: Objects whose value **can be changed** after creation.
	* If you modify a mutable object, it **does not create a new object in memory**, it updates the existing one.

	✅ Examples of mutable data types:

	* `list`
	* `dict`
	* `set`
	* `bytearray`

	👉 Example:

	```python
		a = [1, 2, 3]
		print(id(a))   # memory address before change
		a.append(4)    # modify list
		print(a)       # [1, 2, 3, 4]
		print(id(a))   # memory address remains same
	```

	---

	🔹 **2. Immutable Data Types**

	* **Definition**: Objects whose value **cannot be changed** after creation.
	* If you try to modify an immutable object, **a new object is created in memory**.

	✅ Examples of immutable data types:

	* `int`
	* `float`
	* `complex`
	* `str`
	* `tuple`
	* `frozenset`
	* `bytes`

	👉 Example:

	```python
		x = "hello"
		print(id(x))   # memory address before change
		x = x + " world"  # creates new string
		print(x)       # "hello world"
		print(id(x))   # memory address changes
	```

	---

	🔹 **Key Differences**

	| Feature           | Mutable                                           | Immutable             |
	| ----------------- | ------------------------------------------------- | --------------------- |
	| Can change value? | ✅ Yes                                             | ❌ No                  |
	| Memory address    | Stays same when modified                          | Creates new object    |
	| Examples          | `list`, `dict`, `set`                             | `int`, `str`, `tuple` |
	| Performance       | May be slower (extra memory overhead for changes) | Faster for fixed data |

	---

	✅ **In short**:

	* **Mutable** → can change in place.
	* **Immutable** → cannot change; new object created on modification.

	---
8. What are Python’s type conversion functions?
		
	In Python, **type conversion** means converting a value from one data type to another.
	There are two kinds:

	1. **Implicit Type Conversion (Type Casting by Python / Type Promotion)**

	   * Done automatically by Python.
	   * Python promotes smaller data types to larger data types to avoid data loss.
	   * Example:

	     ```python
	     x = 10      # int
	     y = 2.5     # float
	     z = x + y   # int + float → float
	     print(z, type(z))  # 12.5 <class 'float'>
	     ```

	2. **Explicit Type Conversion (Type Casting by User)**

	   * Done manually using **built-in type conversion functions**.
	   * Common functions:

   | Function        | Converts To     | Example                                    |
   | --------------- | --------------- | ------------------------------------------ |
   | `int(x)`        | Integer         | `int("10") → 10`                           |
   | `float(x)`      | Float           | `float("3.14") → 3.14`                     |
   | `complex(x, y)` | Complex         | `complex(2, 3) → (2+3j)`                   |
   | `str(x)`        | String          | `str(100) → "100"`                         |
   | `list(x)`       | List            | `list((1,2,3)) → [1,2,3]`                  |
   | `tuple(x)`      | Tuple           | `tuple([1,2,3]) → (1,2,3)`                 |
   | `set(x)`        | Set             | `set([1,2,2,3]) → {1,2,3}`                 |
   | `dict(x)`       | Dictionary      | `dict([(1,"a"), (2,"b")]) → {1:'a',2:'b'}` |
   | `frozenset(x)`  | Immutable set   | `frozenset([1,2,3])`                       |
   | `bytes(x)`      | Immutable bytes | `bytes("abc", "utf-8")`                    |
   | `bytearray(x)`  | Mutable bytes   | `bytearray("abc", "utf-8")`                |

	---

	
	You can say:

	> "Python supports both implicit and explicit type conversion.
	> Implicit conversion, also called type promotion, happens automatically when Python converts smaller data types to larger ones to avoid data loss, like converting `int` to `float`.
	> Explicit conversion, or type casting, is done using built-in functions such as `int()`, `float()`, `str()`, `list()`, `tuple()`, `set()`, and so on. These functions allow us to manually convert values from one type to another.
	> For example, `int("10")` converts a string to an integer, and `list((1,2,3))` converts a tuple to a list."

	---

9. How is `None` different from `0`, `False`, and `''`?

	In Python:

	### 🔹 `None`

	* Special constant in Python that represents the **absence of a value** or **no value at all**.
	* Its type is **`NoneType`**.
	* Used commonly as a **default return value** of functions that don’t explicitly return anything.

	```python
	x = None
	print(type(x))   # <class 'NoneType'>
	```

	---

	### 🔹 `0`

	* An **integer numeric value**.
	* Belongs to **`int`** type.
	* Used in arithmetic operations.

	```python
	print(0 + 5)   # 5
	```

	---

	### 🔹 `False`

	* A **Boolean value** (part of `bool` type).
	* Equivalent to `0` in numeric contexts, but semantically different.

	```python
	print(False == 0)   # True
	print(isinstance(False, bool))  # True
	```

	---

	### 🔹 `''` (Empty String)

	* An **empty string** object.
	* Belongs to **`str`** type.
	* Represents a string with length **0**.

	```python
	s = ''
	print(len(s))   # 0
	```

	---


	You can say:

	> "`None` is Python’s special null object that indicates absence of a value.
	> Unlike `0` (an integer), `False` (a Boolean), or `''` (an empty string), which all have actual values of their respective data types, `None` represents the absence of a value.
	> All of them evaluate to `False` in Boolean context, but they are **different in type and meaning**."

---

10. What are Python’s rules for variable naming?
	In Python, variable names must start with a letter or underscore, followed by letters, digits, or underscores. They are case-sensitive, cannot contain spaces or special characters, and must not be keywords. While these are strict rules, Python also follows naming conventions like using underscores for readability and double underscores for special methods.
---

### **3. Operators and Expressions**

11. What are the different types of operators in Python?
	

	✅ **Types of Operators in Python**

	Python supports several categories of operators:

	🔹 1. **Arithmetic Operators**

	- Used for mathematical operations.

	```python
	x, y = 10, 3
	print(x + y)   # 13 (Addition)
	print(x - y)   # 7  (Subtraction)
	print(x * y)   # 30 (Multiplication)
	print(x / y)   # 3.333... (Division → float)
	print(x // y)  # 3 (Floor division → integer)
	print(x % y)   # 1 (Modulus → remainder)
	print(x ** y)  # 1000 (Exponentiation)
	```
	---
	🔹 2. **Comparison (Relational) Operators**

	- Used to compare values → returns `True` or `False`.

	```python
	print(x == y)  # False
	print(x != y)  # True
	print(x > y)   # True
	print(x < y)   # False
	print(x >= y)  # True
	print(x <= y)  # False
	```

	---

	🔹 3. **Assignment Operators**

	- Used to assign values.

	```python
	a = 5
	a += 2   # 7  (a = a + 2)
	a -= 2   # 5  (a = a - 2)
	a *= 3   # 15 (a = a * 3)
	a /= 5   # 3.0
	a %= 2   # 1.0
	a **= 2  # 1.0 (exponent)
	a //= 2  # 0.0 (floor divide)
	```

	---

	 🔹 4. **Logical Operators**

	- Used with Boolean values.

	```python
	print(True and False)  # False
	print(True or False)   # True
	print(not True)        # False
	```

	---

	🔹 5. **Bitwise Operators**

	- Work on binary representation.

	```python
	x, y = 5, 3  # (101, 011 in binary)
	print(x & y)   # 1  (AND → 001)
	print(x | y)   # 7  (OR  → 111)
	print(x ^ y)   # 6  (XOR → 110)
	print(~x)      # -6 (NOT → invert bits)
	print(x << 1)  # 10 (Left shift)
	print(x >> 1)  # 2  (Right shift)
	```

	---

	🔹 6. **Membership Operators**

	= Check if a value exists in a sequence (`list`, `str`, `tuple`, etc.).

	```python
	fruits = ["apple", "banana"]
	print("apple" in fruits)    # True
	print("mango" not in fruits) # True
	```

	---

	 🔹 7. **Identity Operators**

	- Check if two variables point to the **same object in memory**.

	```python
	a = [1,2,3]
	b = a
	c = [1,2,3]
	print(a is b)   # True  (same object)
	print(a is c)   # False (different objects, same values)
	print(a == c)   # True  (values are equal)
	```

	---

	You can say:

	> "Python supports several operators:
	>
	> * Arithmetic (`+`, `-`, `*`, `/`, etc.),
	> * Comparison (`==`, `!=`, `>`, `<`),
	> * Assignment (`=`, `+=`, `-=`),
	> * Logical (`and`, `or`, `not`),
	> * Bitwise (`&`, `|`, `^`, `<<`, `>>`),
	> * Membership (`in`, `not in`), and
	> * Identity (`is`, `is not`).
	>   Arithmetic and comparison operators work on values, logical operators on Boolean expressions, membership checks for presence in sequences, and identity operators check memory reference."

---


12. What is the difference between `is` and `==` operators?
	>"`(==)` checks if two objects have the same value, while is checks if they are the same object in memory.
For example, two lists with identical elements are equal (==), but not identical (is) because they are stored at different memory locations."

13. How does Python handle operator precedence?


| Precedence | Operators                                                               | Associativity   |               |
| ---------- | ----------------------------------------------------------------------- | --------------- | ------------- |
| Highest    | `()` Parentheses                                                        | Left to Right   |               |
|            | `**` Exponentiation                                                     | Right to Left   |               |
|            | `+x`, `-x`, `~x` (Unary plus, minus, bitwise NOT)                       | Right to Left   |               |
|            | `*`, `/`, `//`, `%` (Multiplication, Division, Floor Division, Modulus) | Left to Right   |               |
|            | `+`, `-` (Addition, Subtraction)                                        | Left to Right   |               |
|            | `<<`, `>>` (Bitwise shift)                                              | Left to Right   |               |
|            | `&` (Bitwise AND)                                                       | Left to Right   |               |
|            |`^` (Bitwise XOR)                                                       | Left to Right   |               |
|            | \`                                                                      | \` (Bitwise OR) | Left to Right |
|            | `<`, `<=`, `>`, `>=`, `==`, `!=` (Comparison)                           | Left to Right   |               |
|            | `not` (Logical NOT)                                                     | Right to Left   |               |
|            | `and` (Logical AND)                                                     | Left to Right   |               |
|            | `or` (Logical OR)                                                       | Left to Right   |               |
| Lowest     | `=`, `+=`, `-=`, `*=`, `/=`, etc. (Assignment)                          | Right to Left   |               |

---

### **4. Strings and Collections**

14. What are Python strings? How are they different from lists?

**✅ What is a Python String?**
In Python, a **string** is a sequence of Unicode characters enclosed in single quotes (`'`), double quotes (`"`), or triple quotes (`'''` or `"""`). Strings are **immutable**, meaning once created, their content cannot be changed — any modification creates a new string object in memory. They are widely used for handling textual data such as names, messages, or file contents.


**✅ How is a String Different from a List?**
A **list** is an ordered collection of elements (which can be of different types, such as numbers, strings, or even other lists). Unlike strings, lists are **mutable**, meaning their content can be modified in place — items can be added, removed, or updated without creating a new list object. Also, while strings allow only characters, lists can store heterogeneous data types.

🔹 **Examples**

### String Example (Immutable)

```python
s = "hello"
print(s[0])         # Accessing character → h
# s[0] = "H"       # ❌ Error: strings are immutable
s = s + " world"    # Creates a new string
print(s)            # "hello world"
```

### List Example (Mutable)

```python
lst = [1, 2, 3, "hello"]
print(lst[0])       # Accessing element → 1
lst[0] = 10         # ✅ Lists are mutable
lst.append("world") # Adding new element
print(lst)          # [10, 2, 3, "hello", "world"]
```

---
15. How do slicing and indexing work in Python?
	
	In Python, **indexing** and **slicing** are ways to access elements of sequences like **strings, lists, tuples**.

	* **Indexing** means accessing a single element by its position. Python uses **zero-based indexing**, so the first element has index `0`. Negative indexing is also supported, where `-1` refers to the last element, `-2` to the second last, and so on.

	* **Slicing** means extracting a **subsequence** by specifying a **start index, stop index, and step** using the syntax:

	  ```
	  sequence[start:stop:step]
	  ```

	  * `start` → index to begin (default `0`)
	  * `stop` → index to end **(exclusive)**
	  * `step` → interval (default `1`)

	Slicing is very powerful because it allows copying, reversing, and selecting parts of sequences easily.

	---

	## 🔹 Examples

	### Indexing

	```python
	s = "python"
	print(s[0])   # p (first character)
	print(s[3])   # h (fourth character)
	print(s[-1])  # n (last character)
	print(s[-3])  # h (third from end)
	```

	### Slicing

	```python
	s = "python"
	print(s[0:4])    # "pyth" (from index 0 to 3)
	print(s[2:])     # "thon" (from index 2 to end)
	print(s[:4])     # "pyth" (from start to index 3)
	print(s[::2])    # "pto" (every 2nd character)
	print(s[::-1])   # "nohtyp" (reverse string)
	```

	### On Lists

	```python
	nums = [10, 20, 30, 40, 50]
	print(nums[1])     # 20
	print(nums[-2])    # 40
	print(nums[1:4])   # [20, 30, 40]
	print(nums[::2])   # [10, 30, 50]
	print(nums[::-1])  # [50, 40, 30, 20, 10]
	```

---

16. What is the difference between list, tuple, set, and dictionary?

	In Python, **list, tuple, set, and dictionary** are built-in data structures, but they differ in how they store and manage data:

	* **List** → An ordered, mutable collection that allows duplicates.
	* **Tuple** → An ordered, immutable collection that allows duplicates.
	* **Set** → An unordered collection of unique elements (no duplicates allowed).
	* **Dictionary** → A collection of key–value pairs, where keys are unique and immutable, but values can be duplicated and mutable.

	---

	## 🔹 Examples

	### List (Mutable & Ordered)

	```python
	fruits = ["apple", "banana", "cherry", "apple"]
	fruits.append("mango")   # can add
	print(fruits)            # ['apple', 'banana', 'cherry', 'apple', 'mango']
	```

	### Tuple (Immutable & Ordered)

	```python
	coordinates = (10, 20, 30, 10)
	# coordinates[0] = 50   # ❌ Error: Tuples are immutable
	print(coordinates)       # (10, 20, 30, 10)
	```

	### Set (Mutable & Unordered, No Duplicates)

	```python
	nums = {1, 2, 3, 2, 1}
	nums.add(4)
	print(nums)              # {1, 2, 3, 4}  (no duplicates, unordered)
	```

	### Dictionary (Key–Value Pairs)

	```python
	student = {"name": "Sonu", "age": 21, "age": 22}
	student["course"] = "Python"
	print(student)           # {'name': 'Sonu', 'age': 22, 'course': 'Python'}
	```

	---


	✅ **In short**:

	* Use **list** when you need an ordered collection with modifications.
	* Use **tuple** when you need ordered but fixed data.
	* Use **set** when you need unique items and fast membership checks.
	* Use **dictionary** when you need key–value mappings.

---


17. How is a set different from a frozenset?

	In Python, both **set** and **frozenset** are used to store a collection of **unique, unordered elements**. The key difference lies in **mutability**:

	* **Set** → A mutable collection. You can add, remove, or update elements after creation. Because it’s mutable, sets **cannot be used as dictionary keys** or elements of another set.

	* **Frozenset** → An immutable version of a set. Once created, it **cannot be modified** (no add/remove). Because it’s immutable, frozensets **can be used as dictionary keys** or elements inside another set.

	---

	## 🔹 Examples

	### Set (Mutable)

	```python
	s = {1, 2, 3}
	s.add(4)          # ✅ can add elements
	s.remove(2)       # ✅ can remove elements
	print(s)          # {1, 3, 4}
	```

	### Frozenset (Immutable)

	```python
	fs = frozenset([1, 2, 3])
	# fs.add(4)       # ❌ Error: frozenset has no add()
	print(fs)         # frozenset({1, 2, 3})

	# ✅ Frozenset can be used as a key in dict
	d = {fs: "immutable set"}
	print(d)          # {frozenset({1, 2, 3}): 'immutable set'}
	```


	✅ **In short**:

	* Use **set** when you need a modifiable collection of unique items.
	* Use **frozenset** when you need an immutable, hashable set (e.g., as dictionary keys).

---

### **5. Control Flow**

18. What are Python’s conditional statements?
	In Python, conditional statements allow you to execute specific blocks of code based on conditions. These conditions are usually Boolean expressions (True / False).
 
	 **The main conditional statements in Python are:**

	- `if` → Executes a block of code if the condition is true.
	- `if-else` → Provides an alternative block if the condition is false.
	- `if-elif-else` → Allows multiple conditions to be checked in sequence.
	- Nested `if` → An if statement inside another `if` for more complex conditions.
19. What are Python’s loops (`for`, `while`) and how are they different?

	**`for loop`**
	- Iterates over a sequence (like list, tuple, string, range, etc.).
	- It’s definite iteration (we know how many times it will run).

	**`while loop`**
	- Repeats a block of code as long as a condition is true.
	- It’s indefinite iteration (runs until the condition becomes false, may not know in advance how many times).

20. What are `break`, `continue`, and `pass` statements in Python?

	**`break`**
	- Immediately terminates the loop.
	- Control moves to the first statement after the loop.

	**`continue`**
	- Skips the current iteration of the loop.
	- Control jumps back to the loop condition (next iteration).

	**`pass`**
	- A null statement (does nothing).
	- Used as a placeholder when code is syntactically required but not implemented yet.

---

### **6. Functions**

21. How do you define and call a function in Python?
	A function in Python is a block of reusable code that performs a specific task. Functions help in:
	- Organizing code into smaller, manageable parts.
	- Reusing logic instead of repeating code.
	- Improving readability and maintainability.
	
		In Python, you define a function using the def keyword, and you call it by writing its name followed by parentheses (). Functions can take parameters (inputs) and return values (outputs).

22. What are default arguments, keyword arguments, and arbitrary arguments (`*args`, `**kwargs`)?

	1. **Default Arguments**

	   * Parameters with a default value.
	   * If the caller doesn’t provide a value, the default is used.

	2. **Keyword Arguments**

	   * Arguments are passed by explicitly specifying the parameter name.
	   * Order doesn’t matter when using keywords.

	3. **Arbitrary Arguments**

	   * Used when you don’t know how many arguments will be passed.
	   * `*args` → Collects **positional arguments** into a tuple.
	   * `**kwargs` → Collects **keyword arguments** into a dictionary.

	---

	## 🔹 Examples

	### 1. Default Arguments

	```python
	def greet(name="Guest"):
	    print("Hello,", name)

	greet("Sonu")   # Hello, Sonu
	greet()         # Hello, Guest
	```

	---

	### 2. Keyword Arguments

	```python
	def student(name, age):
	    print("Name:", name, "Age:", age)

	student(age=21, name="Sonu")  
	# Order doesn’t matter → Name: Sonu Age: 21
	```

	---

	### 3. Arbitrary Positional Arguments (`*args`)

	```python
	def add_numbers(*args):
	    return sum(args)

	print(add_numbers(2, 4, 6))      # 12
	print(add_numbers(1, 2, 3, 4, 5))  # 15
	```

	👉 All extra positional arguments are packed into a **tuple**.

	---

	### 4. Arbitrary Keyword Arguments (`**kwargs`)

	```python
	def print_details(**kwargs):
	    for key, value in kwargs.items():
	        print(f"{key}: {value}")

	print_details(name="Sonu", age=21, course="Python")
	```

	**Output:**

	```
	name: Sonu  
	age: 21  
	course: Python
	```



	✅ **In short**:

	* **Default args** → use preset values if not provided.
	* **Keyword args** → specify parameters by name, order doesn’t matter.
	* **`*args`** → many positional args → packed into tuple.
	* **`**kwargs`** → many keyword args → packed into dictionary.

	---




23. What is recursion in Python? Give an example.
	

	**Recursion** in Python (and in general programming) is when a function **calls itself** directly or indirectly to solve a problem.

	A recursive function usually has two key parts:

	1. **Base Case** → Condition that stops recursion (prevents infinite loop).
	2. **Recursive Case** → The function calls itself with a smaller/simpler input.

	Recursion is often used for problems that can be broken into **smaller subproblems** of the same type, such as factorial, Fibonacci, or tree traversal.

	---

	## 🔹 Example 1: Factorial using Recursion

	```python
	def factorial(n):
	    if n == 0 or n == 1:   # Base case
	        return 1
	    else:
	        return n * factorial(n - 1)   # Recursive call

	print(factorial(5))   # 120
	```

	👉 Here:

	* **Base case:** `n == 0 or n == 1` returns `1`.
	* **Recursive case:** `n * factorial(n-1)`.

	---

	## 🔹 Example 2: Fibonacci Series using Recursion

	```python
	def fibonacci(n):
	    if n <= 1:   # Base case
	        return n
	    else:
	        return fibonacci(n-1) + fibonacci(n-2)

	print(fibonacci(6))   # 8
	```

	---




24. What are lambda functions in Python?
	
	In Python, a **lambda function** is a small, anonymous function defined using the `lambda` keyword instead of `def`.

	* **Anonymous** → It has no name (unless assigned to a variable).
	* **Single expression** → Lambda functions can contain only one expression (no statements like loops or assignments).
	* **Return value** → The expression is automatically returned, no `return` keyword needed.

	They’re often used when a short function is needed **temporarily**, especially inside functions like `map()`, `filter()`, `reduce()`, or sorting with `key`.

	---

	## 🔹 Syntax

	```python
	lambda arguments: expression
	```

	---

	## 🔹 Examples

	### 1. Simple lambda function

	```python
	square = lambda x: x * x
	print(square(5))   # 25
	```

	---

	### 2. Multiple arguments

	```python
	add = lambda a, b: a + b
	print(add(3, 7))   # 10
	```

	---

	### 3. Using with `map()`

	```python
	nums = [1, 2, 3, 4]
	squares = list(map(lambda x: x**2, nums))
	print(squares)     # [1, 4, 9, 16]
	```

	---

	### 4. Using with `filter()`

	```python
	nums = [10, 15, 20, 25, 30]
	evens = list(filter(lambda x: x % 2 == 0, nums))
	print(evens)       # [10, 20, 30]
	```

	---

	### 5. Using with `sorted()`

	```python
	students = [("Sonu", 21), ("Monu", 19), ("Krishna", 25)]
	sorted_students = sorted(students, key=lambda x: x[1])
	print(sorted_students)  
	# [('Monu', 19), ('Sonu', 21), ('Krishna', 25)]
	```

	---


	✅ **In short**:
	Lambda functions are **anonymous, one-line functions** created with `lambda`, useful for short tasks like sorting, filtering, and mapping.


---

### **7. Advanced Basics**

25. What are Python modules and packages?
	- In Python, a module is a single file containing Python code (functions, classes, or variables) that can be imported and reused in other programs.
	- A package is a collection of related modules organized in a directory with an __init__.py file (in Python 3.3+, it’s optional) to make it a package.
	- In short, a module is a file, and a package is a folder of modules.
---
26. What is the difference between shallow copy and deep copy?

	When you copy objects in Python, there are two main types: **shallow copy** and **deep copy**.

	* **Shallow Copy**

	  * Creates a new object, but **does not recursively copy nested objects**.
	  * Instead, it only copies references to the inner objects.
	  * So, changes in nested objects affect both copies.
	  * Can be made using `copy.copy()` or slicing (`[:]` for lists).

	* **Deep Copy**

	  * Creates a new object and **recursively copies all nested objects**.
	  * Completely independent copy — changes in nested objects won’t affect the original.
	  * Made using `copy.deepcopy()`.

	---

	## 🔹 Example

	```python
	import copy

	# Original nested list
	original = [[1, 2], [3, 4]]

	# Shallow copy
	shallow = copy.copy(original)

	# Deep copy
	deep = copy.deepcopy(original)

	# Modify nested element
	original[0][0] = 99

	print("Original:", original)   # [[99, 2], [3, 4]]
	print("Shallow:", shallow)     # [[99, 2], [3, 4]]  (affected!)
	print("Deep:", deep)           # [[1, 2], [3, 4]]   (not affected)
	```

	---



	✅ **In short**:

	* **Shallow copy** → Copies outer object, shares nested objects.
	* **Deep copy** → Copies everything recursively, fully independent.

	---


27. What is the difference between local, global, and nonlocal variables?
	
	In Python, variables have different scopes (the region where they can be accessed):

	**`Local Variable`**
	- Defined inside a function.
	- Accessible only within that function.
	- Created when function is called, destroyed when function ends.

	**`Global Variable`**
	- Defined outside all functions.
	- Accessible anywhere in the file, inside or outside functions.
	- To modify a global variable inside a function, you must use the global keyword.

	**`Nonlocal Variable`**
	- Used in nested functions.
	- Refers to a variable in the nearest enclosing (non-global) scope.
	- Declared using nonlocal keyword.

28. What are Python decorators?


29. What are Python generators and iterators?
30. What is the difference between Python 2 and Python 3?

---


