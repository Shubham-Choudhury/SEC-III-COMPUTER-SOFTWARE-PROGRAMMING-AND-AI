---
layout: base
title: "Lecture 11: Python Operators"
date: 2026-06-29 09:00:00 +0530
categories: jekyll update
permalink: "/lecture-11-python-operators/"
---

# {{ page.title | escape }}

## 1. What is an operator?

An operator is a symbol or keyword that performs an operation on one or more values.

## 2. What is an operand?

An operand is the value or variable on which an operator performs an operation.
For example:

$$
10+5=15
$$

- $10$ and $5$ are operands.
- $+$ is the operator.
- $15$ is the result.

## # I. Classification of Python operators

- **Arithmetic operators:** Perform mathematical calculations.

- **Assignment operators:** Assign or update variable values.

- **Comparison operators:** Compare values and return Boolean results.

- **Logical operators:** Combine or reverse logical conditions.

- **Identity operators:** Check whether two references point to the same object.

- **Membership operators:** Check whether a value exists in a collection.

- **Bitwise operators:** Operate on integer bits.

## # I. Arithmetic operators

| Operator | Name           | Example  | Result   |
| -------- | -------------- | -------- | -------- |
| +        | Addition       | 10 + 3   | 13       |
| -        | Subtraction    | 10 - 3   | 7        |
| \*       | Multiplication | 10 \* 3  | 30       |
| /        | Division       | 10 / 3   | 3.333... |
| //       | Floor division | 10 // 3  | 3        |
| %        | Modulus        | 10 % 3   | 1        |
| \*\*     | Exponentiation | 2 \*\* 3 | 8        |

## # II. Assignment operators

### # Simple assignment `(=)`

```python
x = 10
print(x)
```

OUTPUT:

```
10
```

### # Augmented assignment operators

| Operator  | Equivalent expression |
| --------- | --------------------- |
| x += 5    | x = x + 5             |
| x -= 5    | x = x - 5             |
| x \*= 5   | x = x \* 5            |
| x /= 5    | x = x / 5             |
| x //= 5   | x = x // 5            |
| x %= 5    | x = x % 5             |
| x \*\*= 2 | x = x \*\* 2          |

## # III. Comparison (relational) operators

| Operator | Meaning                  | Example | Result |
| -------- | ------------------------ | ------- | ------ |
| ==       | Equal to                 | 5 == 5  | True   |
| !=       | Not equal to             | 5 != 3  | True   |
| >        | Greater than             | 8 > 5   | True   |
| <        | Less than                | 2 < 5   | True   |
| >=       | Greater than or equal to | 5 >= 5  | True   |
| <=       | Less than or equal to    | 3 <= 2  | False  |

## # IV. Logical operators

Python has three main logical operators:

- and
- or
- not

### # The `and` operator

| Condition A | Condition B | A and B |
| ----------- | ----------- | ------- |
| True        | True        | True    |
| True        | False       | False   |
| False       | True        | False   |
| False       | False       | False   |

### # The `or` operator

| Condition A | Condition B | A or B |
| ----------- | ----------- | ------ |
| True        | True        | True   |
| True        | False       | True   |
| False       | True        | True   |
| False       | False       | False  |

### # The `not` operator

Reverses a Boolean condition.

## V. Bitwise operators

| Operator | Name        | Meaning                     |
| -------- | ----------- | --------------------------- |
| &        | AND         | Bit is 1 if both bits are 1 |
| \|       | OR          | Bit is 1 if either bit is 1 |
| ^        | XOR         | Bit is 1 if the bits differ |
| ~        | NOT         | Inverts integer bits        |
| <<       | Left shift  | Shifts bits to the left     |
| >>       | Right shift | Shifts bits to the right    |
