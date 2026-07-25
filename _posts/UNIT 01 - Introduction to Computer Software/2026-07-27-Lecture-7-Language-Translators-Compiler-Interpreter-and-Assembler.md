---
layout: base
title: "Lecture 7: Language Translators – Compiler, Interpreter, and Assembler"
date: 2026-06-29 09:00:00 +0530
categories: jekyll update
permalink: "/lecture-7-language-translators-compiler-interpreter-and-assembler/"
---

# {{ page.title | escape }}

## 1. What is a Programming Language?

A Programming Language is a formal language used to write instructions that tell a computer how to perform a task.

Examples:

- Python
- C
- C++
- Java
- JavaScript
- PHP
- Rust

## 2. Why Can't Computers Understand Python or C?

Computers are made from electronic circuits. Electronic circuits have only two electrical states: `ON`/`OFF`. These states are represented as: `1`/`0`. Therefore, Computers understand only binary instructions.
Example:

- 10110010
- 11100011
- 01010101

Humans cannot easily read binary. Hence, programming languages were invented.

## 3. Evolution of Programming Languages

Programming languages have evolved over time to make programming easier.

![Evolution of Programming Languages]({{ '/assets/images/Evolution-of-Programming-Languages.png' | relative_url }})

## I. First Generation Language

### # Machine Language

Machine Language consists entirely of binary digits (0s and 1s).

#### # Characteristics

- Written in binary.
- Executed directly by CPU.
- Fastest execution.
- Difficult for humans.
- Machine dependent.

#### # Advantages

- Very fast.
- No translator required.
- Direct execution.

#### # Disadvantages

- Difficult to write.
- Difficult to debug.
- Difficult to maintain.
- Error-prone.
- Not portable.

## II. Second Generation Language

### # Assembly Language

Assembly Language uses mnemonic symbols instead of binary numbers.

#### # Example

Instead of 10110001, we write MOV A,B

#### # Common Assembly Instructions

```asm
MOV
ADD
SUB
MUL
DIV
JMP
CMP
```

These are easier for humans to remember.

#### # Characteristics

- Uses symbols.
- Easier than Machine Language.
- Faster execution.
- Machine dependent.
- Requires an Assembler.

#### # Advantages

- Easier than binary.
- Efficient.
- Faster execution.

#### # Disadvantages

- Difficult compared to modern languages.
- Machine dependent.
- Requires knowledge of hardware.

## III. Third Generation Language (3GL)

### # High-Level Language

High-Level Languages use English-like syntax.

#### # Examples

- Python
- C
- C++
- Java
- Pascal
- BASIC

#### # Characteristics

- Human readable.
- Portable.
- Easy to learn.
- Easy debugging.
- Requires translators.

#### # Advantages

- Easy programming.
- Easy maintenance.
- Portable.
- Faster development.

#### # Disadvantages

- Slower than Machine Language.
- Requires compiler or interpreter.

## 4. Comparison of Programming Languages

| Feature             | Machine Language | Assembly Language | High-Level Language                                                        |
| ------------------- | ---------------- | ----------------- | -------------------------------------------------------------------------- |
| Representation      | Binary           | Mnemonics         | English-like                                                               |
| Ease of Programming | Very Difficult   | Moderate          | Easy                                                                       |
| Execution Speed     | Fastest          | Fast              | Slower than machine code                                                   |
| Translator Required | No               | Assembler         | Compiler/Interpreter                                                       |
| Portability         | No               | No                | Yes (source code can often be compiled/interpreted on different platforms) |

## 5. Language Translator

A Language Translator is software that converts source code written in one programming language into machine code that the computer can execute.

### # Types of Language Translators

There are three main types:

![Types of Language Translators]({{ '/assets/images/Types-of-Language-Translators.png' | relative_url }})

### I. Compiler

A Compiler translates the entire source program into machine code before execution.

#### # Characteristics

- Translates the whole program.
- Generates an executable file.
- Reports errors after compilation.
- Faster execution after successful compilation.

#### # Advantages

- Fast execution.
- Optimized code.
- Suitable for large applications.

#### # Disadvantages

- Compilation takes time.
- Must fix compilation errors before execution.

#### # Examples

- GCC (GNU Compiler Collection)
- Clang
- Microsoft Visual C++ Compiler

### II. Interpreter

An Interpreter translates and executes the program one statement at a time.

#### # Characteristics

- No separate executable file.
- Stops when an error occurs.
- Easier debugging.
- Slower execution compared to compiled code.

#### # Advantages

- Easy debugging.
- Immediate execution.
- Platform-independent source code.

#### # Disadvantages

- Slower execution.
- Program must be interpreted each time it runs.

#### # Examples

- Python Interpreter
- Ruby Interpreter

### III. Assembler

An Assembler converts Assembly Language into Machine Language.

#### # Characteristics

- Converts mnemonics into binary.
- Produces machine code.
- Machine dependent.

### # Comparison of Compiler, Interpreter and Assembler

| Feature         | Compiler                | Interpreter             | Assembler               |
| --------------- | ----------------------- | ----------------------- | ----------------------- |
| Input           | High-Level Language     | High-Level Language     | Assembly Language       |
| Translation     | Entire Program          | One Statement at a Time | Entire Assembly Program |
| Output          | Executable Machine Code | Executes Directly       | Machine Code            |
| Speed           | Fast after compilation  | Slower during execution | Fast                    |
| Error Reporting | After compilation       | Line by line            | During assembly process |

## Unit I Mind Map

![Unit I Mind Map]({{ '/assets/images/Unit-I-Mind-Map.png' | relative_url }})
