---
layout: base
title: "Lecture 12: Bitwise Operators in Python"
date: 2026-06-29 09:00:00 +0530
categories: jekyll update
permalink: "/lecture-12-bitwise-operators-in-python/"
---

# {{ page.title | escape }}

## 1. Introduction to bitwise operators

In Python, **bitwise operators perform operations on the individual bits
of integer values**.

Computers store and process information using binary digits:

- `0` represents a bit that is off.
- `1` represents a bit that is on.

Consider the decimal number `13`. Its binary representation is `1101`.

```
    Bit      Place value

      1             8
      1             4
      0             2
      1             1
```

Therefore:

$$
(13)_{10}=1(8)+1(4)+0(2)+1(1)=1101_2
$$

Similarly,

$$
(10)_{10}=1010_2
$$

A bitwise operator compares or modifies the binary bits of these
integers according to its rule.

### Python's six bitwise operators

| Operator | Name        | Purpose                                      |
| -------- | ----------- | -------------------------------------------- |
| `&`      | Bitwise AND | A result bit is 1 when both bits are 1       |
| \|       | Bitwise OR  | A result bit is 1 when at least one bit is 1 |
| `^`      | Bitwise XOR | A result bit is 1 when the bits differ       |
| `~`      | Bitwise NOT | Inverts the bits                             |
| `<<`     | Left shift  | Shifts bits to the left                      |
| `>>`     | Right shift | Shifts bits to the right                     |

## 2. Bitwise AND (`&`)

The AND operator produces `1` only when **both corresponding bits are
1**.

### Truth table

| A   | B   | A & B |
| --- | --- | ----- |
| 0   | 0   | 0     |
| 0   | 1   | 0     |
| 1   | 0   | 0     |
| 1   | 1   | 1     |

### Worked example: `12 & 10`

First, convert both numbers to binary:

```text
12 = 1100
10 = 1010
     ----
     1000
```

The binary result `1000` is (8) in decimal.

```python
print(12 & 10)
```

Output:

```text
8
```

Another example:

```python
a = 7
b = 3
print(a & b)
```

Calculation:

```text
7 = 0111
3 = 0011
    ----
    0011
```

Output: `3`.

### Applications of bitwise AND

- Checking whether a particular bit is set.
- Extracting selected bits from an integer.
- Applying bit masks.
- Working with hardware registers and permissions.

## 3. Bitwise OR (`|`)

The OR operator produces `1` when **at least one of the corresponding
bits is 1**.

### Truth table

| A   | B   | A \| B |
| --- | --- | ------ |
| 0   | 0   | 0      |
| 0   | 1   | 1      |
| 1   | 0   | 1      |
| 1   | 1   | 1      |

### Worked example: `12 | 10`

```text
12 = 1100
10 = 1010
     ----
     1110
```

The result is (8+4+2=14).

```python
print(12 | 10)
```

Output: `14`.

Another example:

```python
a = 5
b = 6
print(a | b)
```

Calculation:

```text
5 = 0101
6 = 0110
    ----
    0111
```

Output: `7`.

### Applications of bitwise OR

OR is useful when we want to **turn selected bits on without changing
other bits**. For example, OR can enable a particular feature in a set
of flags while preserving other enabled features.

## 4. Bitwise XOR (`^`)

XOR stands for **exclusive OR**. It produces `1` when the corresponding
bits are different and `0` when they are the same.

### Truth table

| A   | B   | A ^ B |
| --- | --- | ----- |
| 0   | 0   | 0     |
| 0   | 1   | 1     |
| 1   | 0   | 1     |
| 1   | 1   | 0     |

### Worked example: `12 ^ 10`

```text
12 = 1100
10 = 1010
     ----
     0110
```

```python
print(12 ^ 10)
```

Output: `6`.

### Important XOR properties

**Property 1: XOR with zero**

```python
print(9 ^ 0)  # 9
```

**Property 2: XOR with itself**

```python
print(9 ^ 9)  # 0
```

**Property 3: XOR is commutative**

```python
print(5 ^ 7)  # 2
print(7 ^ 5)  # 2
```

**Property 4: XOR can toggle bits**

Applying XOR with a mask changes each selected bit from `0` to `1` or
from `1` to `0`.

## 5. Bitwise NOT (`~`)

The NOT operator inverts the bits of an integer. At the bit level, `0`
becomes `1` and `1` becomes `0`.

However, Python has an important detail: Python integers have arbitrary
precision, and bitwise NOT follows this identity:

$$
\sim x=-(x+1)
$$

Therefore:

```python
print(~5)
```

Output: `-6`.

Similarly:

```python
print(~0)   # -1
print(~1)   # -2
print(~10)  # -11
```

### Bitwise NOT versus logical NOT

```python
print(~5)
print(not 5)
```

Output:

```text
-6
False
```

- `~5` performs a bitwise inversion of the integer.
- `not 5` performs a logical truth-value test. Since `5` is truthy,
  `not 5` returns `False`.

## 6. Left shift (`<<`)

The left-shift operator moves the bits of an integer to the left by a
specified number of positions.

Syntax:

```python
number << positions
```

For non-negative integers, shifting left by one position is equivalent
to multiplying by 2.

### Example: `5 << 1`

```text
5 = 0101
    << 1
    ----
    1010
```

```python
print(5 << 1)
```

Output: `10`.

### Example: `5 << 2`

```text
5 = 0101
5 << 2 = 10100
```

```python
print(5 << 2)
```

Output: `20`.

## 7. Right shift (`>>`)

The right-shift operator moves the bits to the right.

Syntax:

```python
number >> positions
```

For non-negative integers, shifting right by one position is equivalent
to integer division by 2, discarding the remainder.

### Example: `20 >> 1`

```text
20 = 10100
20 >> 1 = 1010
```

```python
print(20 >> 1)  # 10
```

### Example: `20 >> 2`

```text
20 = 10100
20 >> 2 = 101
```

```python
print(20 >> 2)  # 5
```
