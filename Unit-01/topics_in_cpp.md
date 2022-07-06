---
layout: default
title: Selected Topics in C++
parent: Unit:01 - Compiling concepts
nav_order: 1
---

## What are `INCLUDE_GAURDS`

Include gaurds ensure that the headers are not called more than once during the time of project compilation.

This is very important because it can put out some errors like redeclaration errors when you run without a header gaurd.


Here is an example consider the code.

`Mass.h`
```cpp
#include <iostream.h
```
