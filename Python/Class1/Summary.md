# Python Class Blueprint with Notebook

This project demonstrates the **basic Python concepts required to create a `.pyib` blueprint file and test it interactively using a Jupyter Notebook (`.ipynb`)**.

The repository is designed as a **simple learning environment for Python class fundamentals**, including identifiers, keywords, variables, and object-oriented programming.

---

# 📚 Features

* Python setup and environment verification
* Explanation of identifiers and keywords
* Basic Python variables and data types
* Class and object creation
* Constructor and methods
* `.pyib` blueprint/interface file
* Interactive experimentation with Jupyter Notebook

---

# 🛠 Tech Stack

* Python
* Jupyter Notebook

---

# 📂 Project Structure

```text
python-class-blueprint/
│
├── notebook.ipynb      # Interactive notebook for testing code
├── student.pyib        # Blueprint/interface file
└── README.md           # Project documentation
```

---

# ⚙️ Setup Guide

## 1. Install Python

Download Python from:

https://www.python.org

Verify installation:

```bash
python --version
```

Example output:

```text
Python 3.12.0
```

---

## 2. Install Jupyter Notebook

Install the notebook package using pip:

```bash
pip install notebook
```

Start the notebook server:

```bash
jupyter notebook
```

Your browser will open the notebook interface where you can **run Python code interactively**.

---

# 🐍 Python Basics

## Identifiers

Identifiers are **names given to variables, classes, functions, or objects**.

Example:

```python
name = "Alex"
age = 20
```

### Rules

* Must start with a **letter or underscore**
* Cannot start with a **number**
* Cannot contain **spaces**
* Cannot use **Python keywords**

### Valid Examples

```python
student_name
_total
userID
```

---

# 🔑 Python Keywords

Keywords are **reserved words with predefined meanings in Python**.

### Examples

```text
False
True
None
class
def
if
else
for
while
return
import
```

### Example Usage

```python
class Student:
    pass
```

---

# 📦 Variables and Data Types

Variables store values in memory.

Example:

```python
age = 21
name = "John"
price = 10.5
is_active = True
```

### Common Python Data Types

| Type  | Example         |
| ----- | --------------- |
| int   | 10              |
| float | 10.5            |
| str   | "Hello"         |
| bool  | True            |
| list  | [1,2,3]         |
| dict  | {"name":"Alex"} |

---

# 🧱 Python Classes

A **class is a blueprint for creating objects**.

### Basic Syntax

```python
class ClassName:
    pass
```

### Example

```python
class Student:
    pass
```

---

# 🧍 Creating Objects

Objects are **instances of classes**.

```python
class Student:
    pass

s1 = Student()
```

---

# ⚙️ Constructor

The constructor initializes object attributes.

```python
class Student:

    def __init__(self, name, age):
        self.name = name
        self.age = age
```

Example:

```python
s1 = Student("Alex", 20)
```

---

# 🔧 Methods

Methods are **functions defined inside classes**.

```python
class Student:

    def __init__(self, name):
        self.name = name

    def greet(self):
        print("Hello", self.name)
```

Usage:

```python
s1 = Student("Alex")
s1.greet()
```

---

# 🧩 Example `.pyib` Blueprint

Example blueprint structure:

```python
class StudentInterface:

    def __init__(self, name, age):
        self.name = name
        self.age = age

    def display(self):
        pass
```

This file defines the **expected class structure**.

---

# 📓 Using the Notebook

Open the notebook and test the implementation.

Example cell:

```python
class Student:

    def __init__(self, name, age):
        self.name = name
        self.age = age

    def display(self):
        print(self.name, self.age)


s1 = Student("Alex", 20)
s1.display()
```

Output:

```text
Alex 20
```

---

# 🎯 Learning Goals

This repository helps you understand:

* Python environment setup
* Identifiers and keywords
* Variables and data types
* Python class structure
* Object creation
* Blueprint design using `.pyib`
* Interactive coding using Jupyter Notebook

---

# 🤝 Contributing

Contributions are welcome.

Steps:

```bash
git fork
git clone <repo-url>
git checkout -b feature-branch
```

Submit a **pull request** after making improvements.

---

# 📜 License

This project is licensed under the **MIT License**.
