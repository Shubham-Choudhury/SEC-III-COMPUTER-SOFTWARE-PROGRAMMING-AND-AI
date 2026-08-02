---
layout: base
title: "Lecture 9: Variables, Keywords, Identifiers, Constants, and Data Types in Python"
date: 2026-06-29 09:00:00 +0530
categories: jekyll update
permalink: "/lecture-9-variables-keywords-identifiers-constants-and-data-types-in-python/"
---

# {{ page.title | escape }}

## 1. What is a Variable?

A variable is a named memory location used to store data that can change during program execution.

$$\text{A variable is like a container (box) that stores information.}$$

### # Creating Variables in Python

#### **General Syntax:**

```python
variable_name = value
```

#### Example:

```python
name = "Rahul"
age = 20
cgpa = 8.75
```

### # Understanding the Assignment Operator (=)

In mathematics meaning of `x = 10` is "x is equal to 10." but in Python it means "Store the value 10 inside the variable x."

#### Example:

```python
x = 100
print(x)
```

#### Output:

```
100
```

### # Variable Assignment

```python
city = "Kolkata"
print(city)
```

#### Output:

```
Kolkata
```

### # Multiple Variables

```python
name = "Rahul"
age = 20
marks = 95

print(name)
print(age)
print(marks)
```

#### Output:

```
Rahul
20
95
```

### # Updating Variables

Variables can change during execution.

```python
marks = 80
print(marks)
marks = 95
print(marks)
```

#### Output:

```
80
95
```

The previous value is replaced by the new value.

### # Assigning Multiple Variables

#### Method 1:

```python
x = 10
y = 20
z = 30

print(x)
print(y)
print(z)
```

#### Output:

```
10
20
30
```

#### Method 2:

```python
x, y, z = 10, 20, 30

print(x)
print(y)
print(z)
```

#### Output:

```
10
20
30
```

### # Assigning Same Value

```python
a = b = c = 100

print(a)
print(b)
print(c)
```

#### Output:

```
100
100
100
```

## 2. What are Identifiers?

An identifier is the name given to variables, functions, classes, modules, or other user-defined objects.

#### Examples:

```python
student_name

roll_number

calculate_total

Employee
```

### # Rules for Naming Identifiers

#### **Rule 1:** Must begin with Letter (A–Z or a–z) OR Underscore (\_)

#### CORRECT:

```python
name
_age
student1
```

#### INCORRECT:

```python
1student
```

#### **Rule 2:** Cannot contain spaces.

#### CORRECT:

```python
student_name
```

#### INCORRECT:

```python
student name
```

#### **Rule 3:** Cannot contain special characters.

#### INCORRECT:

```python
marks@
student#
salary$
```

#### **Rule 4:** Python is Case Sensitive.

```python
name = "Rahul"
Name = "Amit"
print(name)
print(Name)
```

OUTPUT:

```
Rahul
Amit
```

These are two different variables.

#### **Rule 5:** Keywords cannot be used as identifiers.

#### INCORRECT:

```python
if = 20
```

Produces a `SyntaxError`.

### # Good Variable Names

```python
student_name
total_marks
average_marks
mobile_number
employee_salary
```

### # Poor Variable Names

These names do not clearly describe their purpose.

```python
a
b
x
temp1
xyz123
```

## 3. Naming Conventions (PEP 8)

Python's style guide (PEP 8) recommends using snake_case for variable and function names.

#### Examples:

```python
student_name
total_marks
average_salary
```

#### Avoid names like:

```python
StudentName
TOTALMARKS
studentName
```

## 4. Keywords

Keywords are reserved words that have predefined meanings in Python. They cannot be used as variable names.

#### Examples:

```python
'False', 'None', 'True', 'and', 'as', 'assert', 'async', 'await', 'break', 'class', 'continue', 'def', 'del', 'elif', 'else', 'except', 'finally', 'for', 'from', 'global', 'if', 'import', 'in', 'is', 'lambda', 'nonlocal', 'not', 'or', 'pass', 'raise', 'return', 'try', 'while', 'with', 'yield'
```

### # Viewing All Keywords

```python
import keyword
print(keyword.kwlist)
```

#### Output:

```
['False', 'None', 'True', 'and', 'as', 'assert', 'async', 'await', 'break', 'class', 'continue', 'def', 'del', 'elif', 'else', 'except', 'finally', 'for', 'from', 'global', 'if', 'import', 'in', 'is', 'lambda', 'nonlocal', 'not', 'or', 'pass', 'raise', 'return', 'try', 'while', 'with', 'yield']
```

## 5. Constants

A constant is a value that is intended not to change during program execution. Python does not enforce constants, but programmers use naming conventions. These are written in uppercase to indicate they should not be modified.

#### Example:

```python
PI = 3.14159
MAX_SPEED = 120
COLLEGE_NAME = "SXCD"
```

## 6. Data Types

A data type specifies the kind of value stored in a variable.

### # Python Built-in Data Types

| Data Type | Description         | Example  |
| --------- | ------------------- | -------- |
| int       | Integer numbers     | 10       |
| float     | Decimal numbers     | 5.75     |
| str       | Text                | "Python" |
| bool      | True/False          | True     |
| NoneType  | Represents no value | None     |

### I. Integer (int)

Stores whole numbers.

```python
age = 20
marks = 95
temperature = -5
```

### II. Float (float)

Stores decimal numbers.

```python
salary = 25000.75
pi = 3.14159
cgpa = 8.82
```

### III. String (str)

Stores text enclosed in quotes. Both single and double quotes are valid.

```python
name = "Rahul"
city = 'Kolkata'
```

### IV. Boolean (bool)

Stores logical values. Only two possible values: `True` or `False`.

```python
is_student = True
is_logged_in = False
```

### V. NoneType

Represents the absence of a value.

```python
result = None
print(result)
```

## 7. Dynamic Typing in Python

Unlike languages such as C or Java, Python does not require you to declare a variable's type explicitly. The same variable can refer to values of different types at different times.

#### Example:

```python
x = 10
print(type(x))
```

#### Output:

```
<class 'int'>
```

#### Later:

```python
x = "Python"
print(type(x))
```

#### Output:

```
<class 'str'>
```

## 8. The type() Function

The `type()` function returns the data type of an object.

#### Example:

```python
a = 10
b = 3.14
c = "Hello"
d = True

print(type(a))
print(type(b))
print(type(c))
print(type(d))
```

#### Output:

```
<class 'int'>
<class 'float'>
<class 'str'>
<class 'bool'>
```
