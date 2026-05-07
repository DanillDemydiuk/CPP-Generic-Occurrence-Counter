# Generic Occurrence Counter Library (C++)

## Description
A versatile C++ utility designed to count occurrences of specific values within datasets of any data type. By utilizing C++ templates, this project demonstrates the "Don't Repeat Yourself" (DRY) principle, providing a single, type-agnostic logic for array analysis.


## Key Technical Features
* **Generic Programming (Templates)**: Implements `template <typename T>` to allow the `countOccurrences` function to handle any data type that supports comparison.
* **Type Flexibility**: Demonstrated support for multiple standard types:
    * **Integers (`int`)**
    * **Floating-point numbers (`double`)**
    * **Characters (`char`)**
* **Pointer-Based Traversal**: Efficiently iterates through memory locations using pointer-to-array logic (`T* array`).
* **Linear Search Complexity**: Implements an $O(n)$ search algorithm to accurately count target elements within a specified range.

## Technical Logic
1. **Template Definition**: The function is defined with a placeholder type `T`, making the logic independent of the specific data being processed.
2. **Comparison Loop**: The program iterates from index $0$ to $size - 1$, comparing each `array[i]` to the provided `value`.
3. **Counter Accumulation**: Each match triggers an increment of the internal `count` variable.
4. **Compile-Time Generation**: When called in `main()`, the compiler automatically generates the specific version of the function for the required type.

## How to Build
1. Requirements: C++ compiler (GCC, Clang, or MSVC).
2. Compilation: `g++ main.cpp -o occurrence_counter`
3. Run: `./occurrence_counter`

## Learning Objectives
* Mastering the syntax and power of C++ Template functions.
* Implementing generic algorithms that minimize code duplication.
* Understanding how the C++ compiler handles template instantiation for different types.
