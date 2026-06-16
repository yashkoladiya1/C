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
