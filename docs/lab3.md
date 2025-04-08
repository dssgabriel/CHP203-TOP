# Lab 3: Memory and data structure layout

Software engineering techniques to improve spatial and temporal data locality in the pursuit of performance.

The code for the exercices is available at [github.com/dssgabriel/TOP-25/lab3](https://github.com/dssgabriel/TOP-25/tree/main/lab3).


## Data structure packing

The goal of this exercice is to improve the layout of the data structures used in the `mesh` code.
We start by packing to reduce its memory footprint.

1. Given the alignment rules imposed on structures/classes by the ISO C and C++ standards, determine how many bytes are
used by the `Cell` structure.

2. Rearrange the layout of the `Cell` structure and delete any unnecessary fields to minimize its memory footprint.
Compute how much memory is saved using the optimized layout.

3. Using Perf, check if there is a change in the number of cache misses between the two structure implementations.

4. Measure the execution time difference between both implementations of the `Cell` structure.


## Array of Structures (AoS) vs. Structure of Arrays (SoA)

Next, we try to improve memory access patterns of the `mesh` code by switching AoS to SoA.

1. Use your prefered tool to determine if the innermost loop in the `Mesh::compute_velocity()` function is correctly
vectorized. You can analyze the assembly directely using a disassembler (e.g. `objdump`), or use tools such as Perf or
[MAQAO](https://maqao.org/documentation.html) ([CQA module](https://maqao.org/documentation/MAQAO.Tutorial.CQA.pdf)).

2. Measure the strong scaling of the current code. Write a small script (can be in bash, Python, R, etc.) to plot the
results.

3. Update the `mesh` code to use SoA instead of AoS.

4. Use the same tools as in question 1 to assert that the change has helped the compiler vectorize the code.

5. Measure the strong scaling of the new code.


---

The rest of this lab is your assignment for next week (in groups of two). Your goal is to improve the performance of a
naive matrix product by tuning array layout and memory access patterns.

For this exercise, we will rely on [Kokkos](https://kokkos.org/kokkos-core-wiki/index.html) and its [Views](https://kokkos.org/kokkos-core-wiki/ProgrammingGuide/View.html),
lightweight multidimensional array containers for C++. We will also leverage Kokkos' parallel constructs to express
portable parallelism.

If you have a GPU (NVIDIA w/ CUDA, AMD w/ HIP, or Intel Arc w/ SYCL), you can also change the Memory/Execution spaces
of the code to trivially make it run on your accelerator (see how [here](https://kokkos.org/kokkos-core-wiki/ProgrammingGuide/ProgrammingModel.html)).


## Array layouts

1. Measure the performance of the naive matrix product and plot the results. You can simply measure its runtime, or
derived metrics such as computational performance (in FLOP/s).   
Conduct a strong scaling study and plot the results too.

2. Try changing the layout of the matrices (e.g. `Kokkos::LayoutRight` to `Kokkos::LayoutLeft`). Do you see any
performance improvement? Which combination gives the best results? Explain why.

3. Repeat the steps of question 1.


## Cache blocking

1. Profile the `matrix-product` code using Perf. Specifically, look at cache misses in the L1 and L3 (LLC) caches.

2. Implement a cache-blocked version of the matrix multiplication to improve the spatial and temporal data locality of
the loop.

3. Assert that your implementation computes the correct result. Update the `CMakeLists.txt` file accordingly.

4. Tune the block dimensions to maximize the performance of your cache-blocked version. Use Perf to assert the
improvements in spatial and temporal locality.

5. Make a final performance and strong scaling study of the code and plot the results. Conclude.

