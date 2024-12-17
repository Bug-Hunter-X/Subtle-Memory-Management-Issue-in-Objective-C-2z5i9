# Subtle Memory Management Issue in Objective-C

This repository demonstrates a common, yet easily overlooked, memory management issue in Objective-C.  The problem lies in how objects are created, owned, and released, potentially leading to memory leaks or unexpected crashes.

## Bug Description
The bug involves improper handling of object ownership within a custom class.  This leads to either prematurely deallocating an object or failing to release it at all, resulting in memory leaks or crashes.

## Reproduction Steps
1. Clone this repository.
2. Build and run the `bug.m` file.
3. Observe the behavior and absence of expected deallocation logs.  Compare this to the behavior of `bugSolution.m`.

## Solution
The solution addresses the ownership issue. By correctly managing the object's lifecycle, we ensure proper memory management.

## Learning Points
This example highlights the critical importance of understanding and correctly applying memory management principles in Objective-C, particularly when working with custom classes and their properties.