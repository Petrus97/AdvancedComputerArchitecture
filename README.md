# Advanced Computer Architecture
This repository contains my solutions to the labs projects of the Advance Computer Architecture(1DT024) course in Uppsala University.
## Overview of the labs
The labs assignments and the bonus assignments have been separated on a different branch for grading purposes.
### 1. Cache Simulation with Pin
The first lab was simulating a cache using the [Pin](https://www.intel.com/content/www/us/en/developer/articles/tool/pin-a-dynamic-binary-instrumentation-tool.html) tool by Intel.<br>
The first part of the assignment was to modify the design of the cache such that it could work as _direct mapped cache_ and _2-way set-associative cache_ with a LRU replacement policy.<br>
The second part of the assignment was to visualise the miss ratio between the two cache designs using the given `radix` program.<br>
The bonus part was to optimize the matrix multiplication taking advantage of the cache design. In this solution blocking has been used.
### 2. Coherence and Memory Models
The first part of the assignent was implementing synchronization mechanisms using the synchronizations primitives.<br>
The second part of the assignment was to implement the same synchronization using different types of locks.
The bonus part was to rewrite the `atomic_counter_lock.cpp` using lockguards. Then to apply less restrictive memory models rather than `sequential consistency` in order to achieve the same results without "slowing down" the program execution allowing the compiler to put less fences in the compiled program.<br>
The last part was to implement the CLH lock.
### 3. Scalability of Gauss-Seidel algorithm
In this lab assignment the requested task was to implement a multithread implementation of the Gauss-Seidel algorithm to solve a linear equation system.<br>
The bonus part were theoretical questions about memory models.
### 4. SIMD
This assignment was implementing an optimized version of three programs(text to lower case, matrix-vector multiplication, matrix-matrix multiplication) using vectorized instructions (SSE 4.1). <br>
The bonus part was to implement a highly optimize version of the matrix-matrix multiplication using _blocking_ and vectorized instructions.