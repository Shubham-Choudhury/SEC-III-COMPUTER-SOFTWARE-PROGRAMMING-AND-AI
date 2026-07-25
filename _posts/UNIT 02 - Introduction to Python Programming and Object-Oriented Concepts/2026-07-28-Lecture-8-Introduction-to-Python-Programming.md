---
layout: base
title: "Lecture 8: Introduction to Python Programming"
date: 2026-06-29 09:00:00 +0530
categories: jekyll update
permalink: "/lecture-8-introduction-to-python-programming/"
---

# {{ page.title | escape }}

## I. What is Python?

Python is a high-level, interpreted, general-purpose programming language known for its simplicity, readability, and versatility.

## II. Features of Python

1. Simple:

   Python syntax resembles English.

   Example:

   ```python
   print("Hello World")
   ```

2. Easy to Learn:

   Python uses fewer keywords and has a clean syntax.

   Example:

   C Language:

   ```c
   #include<stdio.h>
   int main()
   {
       printf("Hello");
       return 0;
   }
   ```

   Python

   ```python
   print("Hello")
   ```

   Python requires much less code.

3. High-Level Language:

   Python hides low-level hardware details. Programmers focus on solving problems rather than managing memory manually.

4. Interpreted Language:

   Python programs are executed by an interpreter.

   Advantages:
   - Easy debugging
   - Immediate execution
   - No separate compilation step in typical usage

5. Object-Oriented:

   Python supports Classes, Objects, Inheritance, Polymorphism, Encapsulation.

6. Portable:

   Python programs can run on Windows, Linux, macOS. Usually with little or no modification.

7. Open Source

   Python is Free, Open Source, Community Developed. Anyone can use and contribute to Python under its open-source license.

8. Large Standard Library

   Python provides many built-in modules.

   Examples:
   - math
   - random
   - datetime
   - os
   - statistics
   - csv
   - json

## III. Applications of Python

1. Web Development:

   Popular Frameworks:
   - Django
   - Flask
   - FastAPI

   Examples:
   - E-commerce websites
   - College portals
   - Blogs
   - APIs

2. Artificial Intelligence:

   Libraries:
   - TensorFlow
   - PyTorch
   - Keras

   Applications:
   - Chatbots
   - Face Recognition
   - Recommendation Systems

3. Machine Learning:

   Libraries:
   - Scikit-learn
   - XGBoost
   - LightGBM

   Applications:
   - Prediction
   - Classification
   - Clustering

4. Data Science:

   Libraries:
   - Pandas
   - NumPy
   - Matplotlib

   Applications:
   - Data Analysis
   - Visualization
   - Business Analytics

5. Automation:

   Python automates repetitive tasks.

   Examples:
   - File Renaming
   - Email Automation
   - Excel Processing
   - Web Scraping

6. Cybersecurity:

   Applications:
   - Network Scanning
   - Password Testing (authorized use only)
   - Log Analysis
   - Security Automation

7. Game Development:

   Libraries:
   - Pygame

   Examples:
   - 2D Games
   - Educational Games

8. Desktop Applications:

   Libraries:
   - Tkinter
   - PyQt
   - Kivy

9. Internet of Things (IoT):

   Python is used with devices like:
   - Raspberry Pi
   - ESP32 (with MicroPython)
   - Sensors
   - Robotics

10. Scientific Computing:

    Libraries:
    - SciPy
    - SymPy

    Applications:
    - Mathematics
    - Physics
    - Engineering

## IV. Writing the First Python Program

### # Program

```python
print("Hello, World!")
```

### `print()`

Built-in function used to display output.

### `"Hello, World!"`

A string (text enclosed in quotes).

### # Output

```
Hello, World!
```

## V. Python Syntax

Syntax refers to the rules for writing Python programs correctly.

### **Rule 1:**

Python statements are written one per line.

Example:

```python
print("A")
print("B")
```

### **Rule 2:**

Python is Case Sensitive.

Correct: `print("Hello")`

Incorrect: `Print("Hello")`

Error: `NameError` because Print and print are different identifiers.

### **Rule 3:**

Keywords cannot be used as variable names.

Incorrect: `if = 10`. This causes a SyntaxError because if is a reserved keyword.

### **Rule 4:**

Use proper parentheses.

Correct: `print("Hello")`

Incorrect: `print("Hello"`

## VI. Python Comments

Comments help explain code.

```python
# This is a comment
print("Hello")
```
