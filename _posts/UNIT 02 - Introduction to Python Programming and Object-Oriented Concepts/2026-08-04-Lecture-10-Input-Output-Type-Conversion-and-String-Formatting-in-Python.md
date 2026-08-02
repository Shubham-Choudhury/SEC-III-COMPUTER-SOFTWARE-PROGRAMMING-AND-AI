---
layout: base
title: "Lecture 10: Input, Output, Type Conversion, and String Formatting in Python"
date: 2026-06-29 09:00:00 +0530
categories: jekyll update
permalink: "/lecture-10-input-output-type-conversion-and-string-formatting-in-python/"
---

# {{ page.title | escape }}

## 1.1 What is Input?

Input is the data entered by the user into a program.

## 1.2 What is Output?

Output is the information displayed by the program after processing the input.

## 2. The `input()` Function

The `input()` function is used to receive data from the user during program execution.

#### **# Syntax:** `variable = input("Message")`

#### # Example-1:

```python
name = input("Enter your name: ")

print(name)
```

#### # Sample Output:

```
Enter your name: Rahul
Rahul
```

#### # Example-2:

```python
city = input("Enter your city: ")

print("City:", city)
```

#### # Output:

```
Enter your city: Kolkata
City: Kolkata
```

### **# NOTE:**

```python
age = input("Enter Age: ")

print(type(age))
```

#### User enters:

```
20
```

#### Output:

```
<class 'str'>
```

Even though the user entered a number, `input()` always returns a string by default.

The keyboard sends characters (text) to the program. Python receives them as a string. If numerical operations are required, we must convert the input.

## 3. Type Conversion

Type conversion is the process of converting one data type into another.

Types of Type Conversion:

<ol type="I">
<li>Implicit Conversion</li>
<li>Explicit Conversion</li>
</ol>

### I. Implicit Conversion

Performed automatically by Python when it is safe to do so.

#### Example:

```python
x = 10
y = 2.5

print(x + y)
```

#### Output:

```
12.5
```

Here, `10` (int) is automatically converted to `10.0` (float).

### II. Explicit Conversion

Performed by the programmer using conversion functions.

#### Examples:

```
int()
float()
str()
bool()
```

### i. int()

Converts to integer.

#### Example:

```
age = input("Enter Age: ")

age = int(age)

print(age)

print(type(age))
```

#### Input:

```
25
```

#### Output:

```
25

<class 'int'>
```

### ii. float()

Converts to decimal numbers.

#### Example:

```python
cgpa = float(input("Enter CGPA: "))

print(cgpa)
```

#### Input:

```
8.85
```

#### Output:

```
8.85
```

### iii. str()

Converts data into strings.

#### Example:

```python
marks = 95

text = str(marks)

print(type(text))
```

#### Output:

```
<class 'str'>
```

### iv. bool()

Converts values to Boolean.

#### Example:

```python
print(bool(10))
```

#### Output:

```
True
```

#### Example:

```python
print(bool(0))
```

#### Output:

```
False
```

#### # Common Boolean Conversions

| Value             | bool() Result |
| ----------------- | ------------- |
| 0                 | False         |
| 1                 | True          |
| -5                | True          |
| "" (empty string) | False         |
| "Hello"           | True          |
| []                | False         |
| [1,2]             | True          |
| None              | False         |

## 4. `print()` Function

The `print()` function displays output on the screen.

#### **# Syntax:** `print(value)`

#### Printing Multiple Values:

```python
name = "Rahul"

age = 20

print(name, age)
```

#### Output:

```
Rahul 20
```

By default, print() separates items with a space.

### # `sep` Parameter:

`sep` specifies the separator between multiple values.

#### Example-1:

```python
print("A", "B", "C", sep="-")
```

#### Output:

```
A-B-C
```

#### Example-2:

```python
print(10, 20, 30, sep=" : ")
```

#### Output:

```
10 : 20 : 30
```

### # `end` Parameter:

By default, `end="\n"`, which moves to the next line.

#### Example:

```python
print("Hello", end=" ")

print("Students")
```

#### Output:

```
Hello Students
```

### # Escape Sequences

Escape sequences begin with a backslash (`\`).

#### New Line:

```python
print("Python\nProgramming")
```

#### Output:

```
Python
Programming
```

#### Tab:

```python
print("Name\tAge")
```

#### Output:

```
Name    Age
```

#### Backslash:

```python
print("C:\\Python")
```

#### Output:

```
C:\Python
```

#### Double Quote:

```python
print("He said \"Hello\"")
```

#### Output:

```
He said "Hello"
```

#### Single Quote:

```python
print('It\'s Python')
```

#### Output:

```
It's Python
```

## 5. String Formatting

Formatting makes output neat and readable.

### # Method 1: Comma

```python
name = "Rahul"

age = 20

print("Name:", name)
print("Age:", age)
```

#### Output:

```
Name: Rahul
Age: 20
```

### Method 2: Old-Style (%) Formatting

```python
name = "Rahul"

age = 20

print("Name: %s Age: %d" % (name, age))
```

#### Output:

```
Name: Rahul Age: 20
```

#### # Common specifiers:

| Specifier | Meaning |
| --------- | ------- |
| `%d`      | Integer |
| `%f`      | Float   |
| `%s`      | String  |

### Method 3: str.format()

```python
name = "Rahul"

age = 20

print("Name: {} Age: {}".format(name, age))
```

#### Output:

```
Name: Rahul Age: 20
```

### Method 4: f-Strings

Introduced in Python 3.6.

```python
name = "Rahul"

age = 20

print(f"Name: {name}, Age: {age}")
```

#### Output:

```
Name: Rahul, Age: 20
```

## 6. Practical Programs

### I. Program-1: Accept Name and Age.
```python
name = input("Enter Name: ")

age = int(input("Enter Age: "))

print(f"Welcome {name}")

print(f"You are {age} years old.")
```

### II. Program-2: Area of Rectangle
```python
length = float(input("Enter Length: "))

width = float(input("Enter Width: "))

area = length * width

print("Area =", area)
```
### Program-3: Simple Interest

#### Formula:
$$ SI = \frac{P \times R \times T}{100} $$

where:
- SI = Simple Interest
- P = Principal amount (initial sum of money)
- R = Annual rate of interest (in percent)
- T = Time period (in years)

```python
principal = float(input("Principal: "))
rate = float(input("Rate: "))
time = float(input("Time: "))

si = (principal * rate * time) / 100

print(f"Simple Interest = {si}")\
```