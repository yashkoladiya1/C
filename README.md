# Learning Embedded C — Foundations

This repository tracks my structural journey into low-level C programming, specifically optimized for transitioning into Embedded Software Engineering. Rather than just writing syntax, the goal is to understand the underlying logic, memory allocation, and compilation mechanics of the C language.

## Project 01: Core C Mechanics (Hello World)

The entry point of this journey focuses on dissecting a foundational C program to analyze exactly what happens when code interface boundaries meet the runtime environment or operating system.

### Source Code (`main.c`)

```c
#include <stdio.h>

int main() {
    printf("Hello world");
    return 0;
}

Learning Variable Initialization

A dedicated space for mastering the core concepts, syntax, and memory mechanics of variable initialization. This repository documents my transition into low-level systems programming, focusing on writing safe, predictable, and optimized code.

---

 2. Core Concepts Covered

### 📋 What is Variable Initialization?
Initialization is the process of assigning an initial value to a variable at the time of its creation. Understanding the difference between defining a variable and initializing it is crucial for preventing undefined behavior and memory bugs.

### 🔍 Types of Initialization
Depending on the programming language, initialization generally falls into these key categories:

* **Uninitialized (The Danger Zone):** Declaring a variable without a value. In lower-level languages like C/C++, this leaves the variable holding "garbage data" from whatever was previously in that memory address.
* **Explicit Initialization:** Directly assigning a specific value upon declaration.
* **Default Initialization:** When the compiler or runtime environment automatically assigns a baseline value (e.g., `0`, `null`, or `false`) to a declared variable.

---

 3. Implementation Examples

### Lower-Level Safety (C / C++)
In systems programming, explicit initialization is essential to avoid critical memory vulnerabilities.

```cpp
// ❌ Dangerous: Uninitialized variable holds random garbage data
int processingSpeed; 

//  Safe: Explicitly initialized at declaration
int maxSubscribers = 0;
