# Python Basics & Object-Oriented Programming (OOP) Guide

A **professional beginner-friendly guide** covering Python installation, core language concepts, and Object-Oriented Programming (OOP). This document is designed to help beginners quickly understand Python fundamentals and start building structured programs.

---

# 📚 Table of Contents

* [Introduction](#introduction)
* [Python Setup](#python-setup)
* [Identifiers in Python](#identifiers-in-python)
* [Keywords in Python](#keywords-in-python)
* [Variables in Python](#variables-in-python)
* [Python Classes](#python-classes)
* [Creating Objects](#creating-objects)
* [Constructors](#constructors)
* [Class vs Instance Attributes](#class-vs-instance-attributes)
* [Methods in Classes](#methods-in-classes)
* [Types of Methods](#types-of-methods)
* [Encapsulation](#encapsulation)
* [Inheritance](#inheritance)
* [Polymorphism](#polymorphism)
* [Indentation in Python](#indentation-in-python)
* [Comments in Python](#comments-in-python)
* [Modules](#modules)
* [Packages](#packages)
* [Complete Example](#complete-example)
* [Quick Summary](#quick-summary)
* [License](#license)

---

# Introduction

Python is a **high-level, interpreted programming language** known for its simplicity and readability. It supports multiple programming paradigms including:

* Procedural Programming
* Object-Oriented Programming
* Functional Programming

This guide focuses on **Python basics and Object-Oriented Programming concepts**.

---

# Python Setup

## Install Python

1. Visit the official website
   [https://python.org](https://python.org)

2. Download **Python 3.13+**

3. During installation enable:

```
✔ Add Python to PATH
```

---

## Verify Installation

Open **Terminal / Command Prompt**

```
python --version
```

Example output:

```
Python 3.13.5 or 3.13+
```

---

## Running Python

### Interactive Mode

```
python
```

### Run Python Script

```
python file.py
```

Example script:

```python
print("Hello World")
```

Output:

```
Hello World
```

---

# Identifiers in Python

Identifiers are **names used to identify variables, functions, classes, modules, or objects**.

Example:

```python
name = "Parikshit"
age = 20
```

Here:

* `name` → identifier
* `age` → identifier

---

## Rules for Identifiers

* Must start with a **letter or underscore**
* Cannot start with a **number**
* Cannot contain **spaces**
* Cannot be **Python keywords**

### Valid Examples

```
studentName
_total
age2
user_id
```

### Invalid Examples

```
2name
student name
class
```

---

# Keywords in Python

Keywords are **reserved words with predefined meanings in Python**.

They cannot be used as identifiers.

### Common Python Keywords

```
False
None
True
and
as
assert
break
class
continue
def
elif
else
except
finally
for
if
import
in
is
lambda
not
or
pass
raise
return
try
while
with
yield

```

Example:

```python
class Student:
    pass
```

---

# Variables in Python

A **variable stores data in memory**.

Example:

```python
x = 10
name = "Parikshit"
```

### Common Data Types

| Type  | Example |
| ----- | ------- |
| int   | 10      |
| float | 10.5    |
| str   | "Hello" |
| bool  | True    |
| list  | [1,2,3] |
| tuple | (1,2,3) |
| dict  | {"a":1} |
| set   | {1,2,3} |

Example:

```python
age = 20
price = 10.5
name = "Alex"
is_active = True
```

---

# Python Classes

A **class is a blueprint used to create objects**.

Example:

```
Class → Car
Objects → BMW, Tesla, Audi
```

### Basic Syntax

```python
class ClassName:
    pass
```

Example:

```python
class Student:
    pass
```

---

# Creating Objects

An **object is an instance of a class**.

Example:

```python
class Student:
    pass

s1 = Student()
```

Here:

* `Student` → class
* `s1` → object

---

# Constructors

Constructors initialize object attributes.

In Python, constructors are defined using `__init__`.

Example:

```python
class Student:

    def __init__(self, name, age):
        self.name = name
        self.age = age
```

Create object:

```python
s1 = Student("Parikshit", 20)
```

---

# Class vs Instance Attributes

## Instance Attributes

Belong to specific objects.

```python
class Student:

    def __init__(self, name):
        self.name = name
```

---

## Class Attributes

Shared across all objects.

```python
class Student:
    school = "ABC School"
```

---

# Methods in Classes

Functions defined inside classes are called **methods**.

Example:

```python
class Student:

    def __init__(self, name):
        self.name = name

    def greet(self):
        print("Hello", self.name)
```

Usage:

```python
s1 = Student("Parikshit")
s1.greet()
```

Output:

```
Hello Parikshit
```

---

# Types of Methods

## Instance Method

Uses object data.

```python
def greet(self):
```

---

## Class Method

Works with class-level data.

```python
@classmethod
def info(cls):
```

---

## Static Method

Independent of object and class state.

Example:

```python
class Math:

    @staticmethod
    def add(a, b):
        return a + b
```

---

# Encapsulation

Encapsulation hides internal data from outside access.

Example:

```python
class Bank:

    def __init__(self):
        self.__balance = 0
```

`__balance` represents a **private variable**.

---

# Inheritance

Inheritance allows a class to **reuse functionality from another class**.

Example:

```python
class Animal:

    def speak(self):
        print("Animal speaks")

class Dog(Animal):
    pass
```

Here `Dog` inherits from `Animal`.

---

# Polymorphism

Polymorphism allows **different objects to respond differently to the same method name**.

Example:

```python
class Dog:
    def sound(self):
        print("Bark")

class Cat:
    def sound(self):
        print("Meow")
```

---

# Indentation in Python

Python uses **indentation to define code blocks** instead of braces.

Correct:

```python
if True:
    print("Hello")
```

Incorrect:

```python
if True:
print("Hello")
```

---

# Comments in Python

Comments explain code.

### Single-line comment

```python
# this is a comment
```

### Multi-line comment

```python
"""
This is a multi line comment
"""
```

---

# Modules

A **module** is a Python file containing code.

Example file:

```
math.py
```

Import module:

```python
import math
```

---

# Packages

A **package** is a collection of Python modules.

Example structure:

```
project/
│
├── main.py
│
└── utils/
    └── helper.py
```

---

# Complete Example

```python
class Student:

    school = "ABC School"

    def __init__(self, name, age):
        self.name = name
        self.age = age

    def display(self):
        print(self.name, self.age)

s1 = Student("Parikshit", 20)
s1.display()
```

Output:

```
Parikshit 20
```

---
# Quick Summary

| Concept       | Meaning                         |
| ------------- | ------------------------------- |
| Identifier    | Name of variable/function/class |
| Keyword       | Reserved word in Python         |
| Variable      | Stores data                     |
| Class         | Blueprint for objects           |
| Object        | Instance of class               |
| Method        | Function inside class           |
| Constructor   | Initializes object              |
| Inheritance   | Reuse parent class              |
| Encapsulation | Hide internal data              |
| Polymorphism  | Same method different behavior  |

---

# License

This repository is provided for **educational purposes**. You are free to use and modify this content for learning and teaching Python programming.

---
