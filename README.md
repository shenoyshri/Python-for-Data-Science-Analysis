# 🐍 Python for Data Science & Analysis

A beginner-to-intermediate Jupyter Notebook covering core Python concepts essential for Data Science and Analysis. This notebook is structured as a hands-on reference guide, demonstrating concepts through practical code examples.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Topics Covered](#topics-covered)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Notebook Structure](#notebook-structure)
- [Key Concepts at a Glance](#key-concepts-at-a-glance)
- [Author](#author)

---

## Overview

This notebook serves as a comprehensive Python reference built from practical exercises. It covers foundational programming concepts — variables, control flow, data structures, functions, and modules — all of which form the bedrock of Data Science and Analysis workflows.

---

## Topics Covered

| # | Topic | Description |
|---|-------|-------------|
| 1 | **OOP – Classes & Objects** | Defining classes, `__init__`, methods, and object instantiation |
| 2 | **Variables & Data Types** | Strings, integers, floats, type casting, and f-strings |
| 3 | **User Input** | Taking and processing input using `input()` |
| 4 | **Variable Swapping** | Swapping with temp variable and Pythonic tuple unpacking |
| 5 | **Loops** | `for` loops, `while` loops, nested loops, `break`, `continue` |
| 6 | **Pattern Printing** | Triangle and number patterns using nested loops |
| 7 | **Conditional Logic** | `if`, `elif`, `else` statements with real-world use cases |
| 8 | **String Methods** | `.split()`, `.casefold()`, `.find()`, `len()`, slicing |
| 9 | **Lists** | Indexing, slicing, iteration, `range()` |
| 10 | **Dictionaries** | Nested dicts, `.keys()`, `.values()`, sorting, iteration |
| 11 | **Sets** | `pop()`, `add()`, `copy()`, `max()`, `min()`, `difference()`, intersection |
| 12 | **Functions** | Defining functions, parameters, return values, `*args` |
| 13 | **Recursion** | Recursive sum of a list, Fibonacci series |
| 14 | **Built-in Modules** | `datetime`, `random`, `math` |
| 15 | **Custom Modules** | Creating and importing user-defined modules |
| 16 | **Memory & Singletons** | Python object caching, `id()`, singleton behavior for `int`, `bool`, `None` |

---

## Prerequisites

- Python 3.x
- Jupyter Notebook or JupyterLab

Install dependencies:

```bash
pip install jupyter
```

Optional (for notebook extensions):

```bash
pip install jupyter_contrib_nbextensions
jupyter contrib nbextension install --user
```

---

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/shenoy-GitHub/<repo-name>.git
   cd <repo-name>
   ```

2. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

3. **Open the notebook:**
   Navigate to `Python_4_Data_Science_and_Analysis.ipynb` in the Jupyter interface.

---

## Notebook Structure

```
Python_4_Data_Science_and_Analysis.ipynb
│
├── Classes & Objects
│   └── Person class with attributes and display method
│
├── Variables, F-strings & Type Casting
│   └── String formatting, int/float conversion
│
├── User Input & Billing System
│   └── Student record system, supermarket billing simulation
│
├── Loops & Patterns
│   ├── Sum of even numbers up to 50
│   ├── First 20 squares
│   ├── Sum of first 10 odd numbers
│   ├── Numbers divisible by 8 and 12
│   └── Triangle pattern printing
│
├── String Methods
│   └── split, casefold, find, slicing
│
├── Lists & Iteration
│   └── Marvel heroes list with for/while loop examples
│
├── Dictionaries
│   ├── Employee nested dictionary
│   ├── Squares dictionary (1–15)
│   └── Sorting by keys and values
│
├── Sets
│   └── Set operations: union, intersection, difference
│
├── Functions
│   ├── Addition, area of rectangle
│   ├── Max of three numbers
│   ├── Prime number checker
│   ├── Sum of list (iterative + recursive)
│   └── Fibonacci series (recursive)
│
└── Modules
    ├── datetime – current time, day/month formatting
    ├── random – randint, choice
    ├── math – sqrt, cbrt, pow, abs
    └── Custom module import (demo)
```

---

## Key Concepts at a Glance

### 🔹 OOP Example
```python
class Person:
    def __init__(self, name, age, address):
        self.name = name
        self.age = age
        self.address = address

    def display(self):
        print(f"Name: {self.name}\nAge: {self.age}\nAddress: {self.address}")

p = Person("Srikanth", 37, "Udupi")
p.display()
```

### 🔹 Fibonacci (Recursion)
```python
def fibs(num):
    if num == 1:
        return 0
    elif num == 2:
        return 1
    else:
        return fibs(num - 1) + fibs(num - 2)
```

### 🔹 Singleton & Object Caching
```python
# Python caches small integers — same id every time
ids = {id(10) for i in range(5000)}
print(ids)  # Only one unique id

# Strings like "1000" are not cached
ids = {id(int("1000")) for i in range(5000)}
print(ids)  # Multiple unique ids
```

---

## Author

**Srikanth Shenoy**
Data Analyst skilled in SQL, Python, Power BI, and Tableau

- 🔗 [GitHub](https://github.com/shenoy-GitHub)
- 🔗 [LinkedIn](https://www.linkedin.com/in/srikanth-shenoy)

---

> 💡 **Note:** Some cells in this notebook use `input()` for interactive exercises. When running the full notebook, these cells will pause and wait for user input. Run them individually for the best experience.
