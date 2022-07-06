---
layout: default
title: Compiler
parent: Unit:01 - Compiling concepts
nav_order: 2
---

# Compiler (`c++`)
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## What is a compiler ?

A compiler is a program which can translate a block of code written with specific syntax (like `c++` or `Java`) to machine code or which can be readily be executed by the microprocessors of the device.

In computing, a compiler is a computer program that translates computer code written in one programming language into another language.

In what follows `g++` compiler is what I would be using.

A compiler is a special program that translates a programming language's source code into machine code, byte code or another programming language. The source code is typically written in a high level, human-readable language such as `Java` or `c++`

---

## Stages of Compiling

There are three different stages of compiling.

+ Syntactical and semantical checks

  ```bash
    g++ -c input.cpp -I$INCLUDE_DIR -L$LIBRARY_DIR
  ```

+ Assembling the source

  ```bash
    g++ -S input.cpp -I$INCLUDE_DIR -L$LIBRARY_DIR
  ```

+ Conversion to Machine executable and linking binaries
  ```bash
    g++ -o output.out input.cpp -I$INCLUDE_DIR -L$LIBRARY_DIR
  ```

---

### Frequently used flags

+ `-W` Flags:

  + `-Wall` - Checks for warning too

  + `-Werr` - Break if there is a warning

+ `-l` Flag:

  + Linking library. All the library that has to be included during the compilation process

+ `-fPIC` flag:

  + Used to make shared libraries

+ `-std` Flag:

  + The `c++` std that is to be used during compilation

+ `-O` Flag:

  + Optimization flags

+ `-pthread` Flag:

  + Number of threads to be Used

+ `-v` Flag:

  + Verbosity flag

## Example of a simple compilation

## Example with a `.h` file

## Example with multiple `src` files and multiple `header` files

## Example of using `shared library` in compilation

## Example of making a `shared library`
