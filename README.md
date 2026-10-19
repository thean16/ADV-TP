# Advanced Programming for Data Science

Welcome to my repository for **Advanced Programming for Data Science**.

This repository is used to organize my practical work, coding exercises, assignments, TP labs, notes, datasets, and small projects throughout the course.

The main goal of this course is to improve my programming skills and learn how to apply Python to Data Science problems.

---

# Course Overview

| Item | Description |
|---|---|
| Course | Advanced Programming for Data Science |
| Programming Language | Python |
| Field | Programming and Data Science |
| Main Goal | Improve programming skills for Data Science |
| Repository Purpose | Organize course work and track learning progress |

During this course, I want to learn how to write programs that are:

- Clear
- Reusable
- Organized
- Easy to understand
- Easy to test
- Easy to debug
- Easy to maintain

---

# My Learning Objectives

By the end of this course, I want to be able to:

1. Write clean and readable Python code.
2. Understand important Python programming concepts.
3. Use functions, modules, and packages correctly.
4. Understand Object-Oriented Programming.
5. Work with files and datasets.
6. Use NumPy for numerical operations.
7. Use Pandas for data manipulation.
8. Clean and transform data.
9. Create useful data visualizations.
10. Debug Python programs.
11. Test my code.
12. Understand basic code performance.
13. Organize a Data Science project properly.
14. Build a small Data Science application.

---

# Repository Structure

```text
ADV-tp/
│
├── README.md
│
├── TP_01.md
│
├── TP_02.md
│
├── TP_03.md
│
├── TP_04.md
│
├── assignments/
│
├── datasets/
│
├── practice/
│   ├── python/
│   ├── numpy/
│   ├── pandas/
│   └── oop/
│
├── projects/
│
└── notes/
```

Each folder has a specific purpose so that my work is easier to organize and review.

---

# Main Topics

## 1. Python Fundamentals

Before learning advanced concepts, I need to understand the main Python basics.

Topics include:

- Variables
- Data types
- Lists
- Tuples
- Dictionaries
- Sets
- Conditions
- Loops
- Functions
- Input and output

Example:

```python
def calculate_average(values):
    return sum(values) / len(values)


scores = [75, 80, 90]

average_score = calculate_average(scores)

print(average_score)
```

Output:

```text
81.66666666666667
```

---

# 2. Functions

Functions help us organize code into reusable blocks.

Example:

```python
def add(a, b):
    return a + b


result = add(5, 3)

print(result)
```

Output:

```text
8
```

Instead of writing the same code many times, we can create a function and reuse it.

---

# 3. Object-Oriented Programming

Object-Oriented Programming helps us organize programs using classes and objects.

Important concepts include:

- Class
- Object
- Attribute
- Method
- Constructor
- Encapsulation
- Inheritance
- Polymorphism

Example:

```python
class Student:
    def __init__(self, name, score):
        self.name = name
        self.score = score

    def show_result(self):
        print(f"{self.name}: {self.score}")


student = Student("Student A", 85)

student.show_result()
```

Output:

```text
Student A: 85
```

---

# 4. Modules and Packages

A module is a Python file containing reusable code.

Example:

```text
calculator.py
```

Inside the file:

```python
def add(a, b):
    return a + b
```

We can use it from another Python file:

```python
import calculator

print(calculator.add(5, 2))
```

A package is a folder containing related Python modules.

Example:

```text
data_tools/
│
├── __init__.py
├── cleaning.py
├── analysis.py
└── visualization.py
```

This helps make large projects easier to organize.

---

# 5. Clean Code

Writing code that works is important, but writing code that is easy to understand is also important.

Poor example:

```python
a = 10
b = 5
c = a * b
```

Better example:

```python
price = 10
quantity = 5
total_price = price * quantity
```

The second version is easier to understand because the variable names explain their purpose.

---

# 6. PEP 8 Style

PEP 8 provides common recommendations for writing readable Python code.

Some important rules are:

```text
Variables → snake_case

Functions → snake_case

Classes → PascalCase

Constants → UPPERCASE

Indentation → 4 spaces
```

Example:

```python
student_name = "Student A"

MAX_SCORE = 100


def calculate_score():
    pass


class StudentProfile:
    pass
```

Following a consistent style makes code easier to read.

---

# 7. Exception Handling

Errors can happen while a program is running.

Python provides exception handling to manage these problems.

Important keywords:

```text
try
except
else
finally
raise
```

Example:

```python
try:
    number = int(input("Enter a number: "))
    print(100 / number)

except ValueError:
    print("Please enter a valid integer.")

except ZeroDivisionError:
    print("The number cannot be zero.")
```

Exception handling helps prevent the program from stopping unexpectedly.

---

# 8. NumPy

NumPy is useful for numerical computing.

Important topics include:

- Arrays
- Dimensions
- Shape
- Indexing
- Slicing
- Broadcasting
- Statistical functions
- Matrix operations

Example:

```python
import numpy as np


values = np.array([10, 20, 30, 40])

print(np.mean(values))
print(np.max(values))
```

---

# 9. Pandas

Pandas is an important library for working with structured data.

Important topics include:

- Series
- DataFrame
- Reading CSV files
- Selecting columns
- Filtering rows
- Missing values
- Sorting
- GroupBy
- Merge
- Aggregation

Example:

```python
import pandas as pd


df = pd.read_csv("data.csv")

print(df.head())
print(df.info())
print(df.describe())
```

---

# 10. Data Cleaning

Before analyzing data, we often need to clean it.

A simple workflow is:

```text
Raw Data
   ↓
Understand the Dataset
   ↓
Check Missing Values
   ↓
Check Duplicates
   ↓
Fix Data Types
   ↓
Handle Outliers
   ↓
Clean Categories
   ↓
Final Dataset
```

Common cleaning tasks include:

- Missing values
- Duplicate rows
- Incorrect data types
- Outliers
- Text cleaning
- Date conversion
- Category formatting

---

# 11. Data Visualization

Visualization helps us understand data more clearly.

A common Python library is:

```python
import matplotlib.pyplot as plt
```

Some common chart types are:

- Line chart
- Bar chart
- Histogram
- Scatter plot
- Box plot

Before creating a graph, I should ask:

1. What do I want to understand?
2. Which variables do I need?
3. Which graph is best for showing the result?

---

# 12. Debugging

Debugging means finding and fixing problems in code.

My debugging process is:

```text
Read the error message
        ↓
Find the problem
        ↓
Understand the error
        ↓
Check variable values
        ↓
Fix one part
        ↓
Run the program again
```

Common Python errors include:

```text
SyntaxError
TypeError
ValueError
IndexError
KeyError
NameError
FileNotFoundError
```

---

# 13. Testing

Testing helps confirm that the program works correctly.

Example:

```python
def multiply(a, b):
    return a * b


assert multiply(2, 3) == 6
assert multiply(5, 4) == 20
```

Testing is important because code should not only run once successfully.

It should also continue working when we change or improve the program.

---

# 14. Code Performance

A program should not only be correct.

We should also consider how efficiently it works.

Important things to compare include:

- Execution time
- Memory usage
- Number of operations
- Readability

Basic performance concepts include:

```text
O(1)
O(log n)
O(n)
O(n log n)
O(n²)
```

These concepts help describe how a program performs when the amount of data becomes larger.

---

# Data Science Programming Workflow

A simple workflow I can follow is:

```text
Understand the Problem
        ↓
Get the Data
        ↓
Load the Data
        ↓
Explore the Data
        ↓
Clean the Data
        ↓
Transform the Data
        ↓
Analyze the Data
        ↓
Visualize the Results
        ↓
Build a Model if Needed
        ↓
Evaluate
        ↓
Explain the Result
```

Programming is used throughout this process.

---

# TP / Lab Workflow

For each TP, I will try to follow this process:

```text
Read the TP
     ↓
Understand the Objective
     ↓
Understand the Concepts
     ↓
Write the Code
     ↓
Run the Program
     ↓
Check the Output
     ↓
Fix Errors
     ↓
Improve the Code
     ↓
Save the Final Work
```

For each TP, I can record:

```text
TP:
Topic:
Objective:
Main Concepts:
Code:
Output:
Problems:
Solutions:
What I Learned:
```

---

# TP Progress

| TP | Topic | Status |
|---|---|---|
| TP01 | Python Foundations and Clean Coding | 🟡 In Progress |
| TP02 | To be added | ⬜ Not Started |
| TP03 | To be added | ⬜ Not Started |
| TP04 | To be added | ⬜ Not Started |

Progress status:

```text
⬜ Not Started
🟡 In Progress
✅ Completed
```

---

# My Study Method

For every new topic, I will try to follow these steps:

```text
1. Read the concept
2. Understand the meaning
3. Look at a simple example
4. Write the code myself
5. Run the program
6. Change the example
7. Observe the result
8. Create and fix errors
9. Explain what the code does
10. Practice again
```

My goal is not only to make the program run.

I also want to understand:

- What the code does
- Why it works
- When to use it
- What problems can happen
- How to improve it

---

# Current Focus

My current focus is:

```text
Python Foundations
        ↓
Clean Code
        ↓
PEP 8
        ↓
Functions
        ↓
Classes and Objects
        ↓
Modules and Packages
        ↓
Exception Handling
        ↓
Debugging
        ↓
Testing
```

After building a strong Python foundation, I can continue with NumPy, Pandas, Data Cleaning, Visualization, and other Data Science topics.

---

# Final Goal

By the end of this course, I want to be able to take a programming or Data Science problem and solve it step by step.

My target process is:

```text
Understand the Problem
        ↓
Plan the Solution
        ↓
Organize the Project
        ↓
Write Clean Python Code
        ↓
Process the Data
        ↓
Test and Debug
        ↓
Improve the Solution
        ↓
Explain the Result
```

> My final goal is not only to write working code, but also to understand, organize, test, improve, and explain my code independently.