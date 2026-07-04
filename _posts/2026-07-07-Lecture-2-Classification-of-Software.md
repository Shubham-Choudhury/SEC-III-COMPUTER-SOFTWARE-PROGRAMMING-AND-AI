---
layout: base
title: "Lecture 2: Classification of Software"
date: 2026-06-29 09:00:00 +0530
categories: jekyll update
permalink: "/lecture-2-classification-of-software/"
---

# {{ page.title | escape }}

## 1. What is Software Classification?

Software classification is the process of grouping software based on the functions it performs.

### # Types of Software

Software can be broadly classified into the following categories:

![Basic Functions of a Computer]({{ '/assets/images/Types-of-Software.png' | relative_url }})

## I. System Software

System software is software that manages the computer's hardware and provides a platform for application software to run. Without system software, the computer cannot function properly.

### # Functions of System Software

- Controls hardware devices.
- Manages memory.
- Manages CPU scheduling.
- Handles input and output devices.
- Provides a platform for application software.
- Manages files and storage.

## # Components of System Software

System software mainly includes:

- Operating System
- Device Drivers
- Language Translators
- System Utilities

### # Operating System (OS)

The operating system acts as an interface between the user and the computer hardware.

Examples:

- Windows 11
- Ubuntu Linux
- macOS
- Android
- iOS

### # Device Drivers

A device driver is software that enables the operating system to communicate with hardware devices.

Examples:

- Printer Driver
- Graphics Driver
- Audio Driver
- Wi-Fi Driver

### # Language Translators

Language translators convert programs written in programming languages into machine language.

Examples:

- Compiler
- Interpreter
- Assembler

## II. Application Software

Application software is software designed to help users perform specific tasks. Unlike system software, it is user-oriented.

### # Types of Application Software

1. General Purpose Software

   Used by many users for common tasks.

   Examples:
   - Word Processor
   - Spreadsheet
   - Presentation Software
   - Web Browser

2. Specific Purpose Software

   Designed for a particular organization or task.

   Examples:
   - Hospital Management System
   - Banking Software
   - Railway Reservation System
   - Payroll Management System
   - College Management System
   - Library Management System

## III. Utility Software

Utility software is software designed to maintain, optimize, protect, and improve the performance of a computer system. Utility software is sometimes considered a part of system software because it supports system maintenance.

### # Functions

- Improves system performance.
- Removes unnecessary files.
- Protects against viruses.
- Compresses files.
- Backs up important data.
- Optimizes storage.

#### **Examples:**

1. Antivirus Software: Protects against malware and viruses.

   Example:
   - Windows Defender
   - Avast
   - Quick Heal
   - Norton Antivirus

2. Disk Cleanup: Removes temporary files and unnecessary data.

3. Disk Defragmenter: Rearranges fragmented files (mainly for HDDs) to improve performance.

4. Backup Software: Creates copies of important files.
   Examples:
   - Windows Backup
   - Google Drive Backup
   - OneDrive

5. File Compression Software: Reduces file size.

   Examples:
   - WinZip
   - WinRAR
   - 7-Zip

## IV. Firmware

Firmware is a special type of software permanently stored in non-volatile memory (such as ROM or Flash memory) that controls the basic operation of hardware devices. Unlike application software, firmware is closely tied to the hardware.

### # Characteristics

- Stored in ROM or Flash memory.
- Starts when the device is powered on.
- Controls low-level hardware functions.
- Updated only occasionally.

#### **Examples:**

- BIOS (Basic Input/Output System)
- UEFI Firmware
- Router Firmware
- Smart TV Firmware
- Washing Machine Firmware
- Microwave Oven Firmware

## V. Middleware

Middleware is software that acts as a bridge between different software applications or between applications and databases. It enables communication and data exchange between different systems.

### # Why is Middleware Needed?

Different applications may be developed using different programming languages, operating systems, or databases. Middleware allows these systems to work together.

#### **Examples:**

- Database Connectivity (ODBC, JDBC)
- Web Servers
- Application Servers
- Message Brokers
- API Gateways

## Comparison of Software Types

| Feature           | System Software                       | Application Software | Utility Software                   | Firmware                         | Middleware                             |
| ----------------- | ------------------------------------- | -------------------- | ---------------------------------- | -------------------------------- | -------------------------------------- |
| Purpose           | Manages hardware and system resources | Performs user tasks  | Maintains and optimizes the system | Controls hardware at a low level | Connects different software systems    |
| User Interaction  | Indirect                              | Direct               | Indirect                           | Usually none                     | Usually none                           |
| Installed by User | Usually pre-installed                 | Yes                  | Yes                                | Pre-installed                    | Installed by developers/administrators |
| Examples          | Windows, Linux                        | MS Word, Chrome      | Antivirus, Backup                  | BIOS, Router Firmware            | JDBC, Web Server                       |

## Software Stack in a Computer

![Software Stack in a Computer]({{ '/assets/images/Software-Stack-in-a-Computer.png' | relative_url }})
