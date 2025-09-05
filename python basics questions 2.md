# 1. Python Fundamentals

**Q1. Difference between compiled and interpreted languages**:
Compiled languages translate the entire source code into machine code before execution, producing an executable file (e.g., C, C++). Interpreted languages, like Python, execute code line by line using an interpreter, making them slower but easier to debug and platform-independent.

**Q2. Is Python case-sensitive?**
Yes, Python is case-sensitive. Variable names, function names, and identifiers with different cases (e.g., `Var`, `var`, `VAR`) are treated as distinct.

**Q3. Use of indentation in Python**:
Indentation in Python defines code blocks instead of braces `{}` as in other languages. Consistent indentation is mandatory and indicates scope, such as inside loops, conditionals, and functions.

**Q4. Modes of execution in Python**:
Python can run in two modes: **interactive mode**, where commands are executed line by line in the Python shell, and **script mode**, where code is written in a `.py` file and executed as a program.

**Q5. Difference between statement and expression**:
A statement is a complete instruction (e.g., `x = 5`, `if x > 2:`), whereas an expression is a combination of values and operators that produces a result (e.g., `2 + 3` or `x * 10`).
```python
	# Statement example
	x = 10        # assignment statement
	if x > 5:     # conditional statement
	    print("x is greater than 5")

	# Expression example
	y = 2 + 3     # '2 + 3' is an expression
	z = x * 2     # 'x * 2' is an expression

```

---

### 2. Numbers and Operators

**Q1. Difference between `/`, `//`, and `%`**:
- The `/` operator performs floating-point division, returning a decimal result. 
- The `//` operator performs floor division, returning the integer quotient. 
- The `%` operator gives the remainder of a division.

**Q2. Difference between int, float, and complex types**:
An `int` represents whole numbers, a `float` represents decimal numbers with fractional parts, and a `complex` represents numbers with a real and imaginary part (e.g., `3+4j`).

**Q3. Type casting in Python**:
Type casting is converting one data type into another, such as using `int("10")` to convert a string to an integer, or `float(5)` to convert an integer to a float.

**Q4. Difference between round() and math.floor()**:
- `round()` returns the nearest integer, rounding up or down depending on the decimal part.
-  while `math.floor()` always returns the largest integer less than or equal to the number.

**Q5. Handling very large integers**:
Python supports arbitrarily large integers natively. Unlike some languages with fixed-size integer limits, Python automatically adjusts memory to accommodate large values without overflow.

---

### 3. Strings

**Q1. Raw strings in Python**:
Raw strings are prefixed with `r` and treat backslashes (`\`) as literal characters, useful for file paths and regex patterns.

**Q2. String immutability**:
Strings in Python are immutable, meaning once created, their content cannot be modified. Any operation that changes a string actually creates a new string.

**Q3. String formatting methods**:
Python allows string formatting using `%` placeholders, `.format()` method, and modern f-strings (`f"{value}"`), which provide readable and efficient ways to insert values into strings.

**Q4. Reversing a string**:
A string can be reversed using slicing with `[::-1]`, which creates a new string with characters in reverse order.

**Q5. Difference between find() and index()**:
Both search for a substring, but `find()` returns `-1` if not found, while `index()` raises a `ValueError` when the substring is missing.

---

### 4. Lists and Tuples

**Q1. Adding, removing, and updating elements in a list**:
Elements can be added using `append()` or `insert()`, removed with `remove()` or `pop()`, and updated by directly assigning a new value to an index.

**Q2. Difference between append() and extend()**:
`append()` adds a single element (including a list as one element), while `extend()` iterates through another iterable and adds each element individually to the list.

**Q3. List comprehension**:
List comprehension is a concise way to create lists using an expression inside square brackets, often combined with loops or conditions. Example: `[x*x for x in range(5)]` creates `[0, 1, 4, 9, 16]`.

**Q4. Tuples containing mutable objects**:
Although tuples themselves are immutable, they can contain mutable objects like lists, whose contents can be modified.

**Q5. Convert between list and tuple**:
A list can be converted to a tuple using `tuple(list_name)` and a tuple can be converted to a list using `list(tuple_name)`.

---

### 5. Sets and Dictionaries

**Q1. Dictionary keys and values**:
In a dictionary, keys are unique identifiers, and values are the associated data. Keys must be immutable, such as strings, numbers, or tuples.

**Q2. Can a dictionary key be mutable?**
No, dictionary keys must be immutable, because their hash value is used for fast lookups. Mutable objects like lists or sets cannot be used as keys.

**Q3. Difference between dict.get() and normal indexing**:
Using `dict[key]` raises a `KeyError` if the key doesn’t exist, while `dict.get(key)` returns `None` (or a specified default value) instead.

**Q4. Set operations**:
Sets support mathematical operations like union (`|`), intersection (`&`), and difference (`-`), allowing efficient handling of unique elements.

**Q5. Removing duplicates from a list with a set**:
Since sets only store unique elements, converting a list into a set removes duplicates, though it does not preserve order.

---

### 6. Functions and Scope

**Q1. Difference between a function and a method**:
A function is a block of reusable code defined independently, while a method is a function associated with an object and called using dot notation, often operating on that object’s data.

**Q2. Docstrings in Python**:
Docstrings are special strings written inside triple quotes at the start of a function, class, or module to describe its purpose, and they can be accessed using the `__doc__` attribute or `help()` function.
```python
	def add(a, b):
	    """
	    This function takes two numbers as input
	    and returns their sum.
	    """
	    return a + b

	print(add.__doc__)   # Accessing the docstring
	help(add)            # Displays docstring with function signature

```

**Q3. Variable scope and LEGB rule**:
Python follows the LEGB (Local, Enclosing, Global, Built-in) rule to resolve variable names, meaning it first checks inside the current function, then enclosing functions, then global scope, and finally built-in names.

**Q4. Anonymous functions**:
Anonymous functions, also known as lambda functions, are small, unnamed functions defined with the `lambda` keyword, typically used for short, throwaway operations.

**Q5. Difference between return and yield**:
- `return` ends a function and sends a value back.
- `yield` produces a generator, returning values one at a time and pausing the function state between calls for memory-efficient iteration.

---


