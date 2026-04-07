# Home

This site contains lectures and practical work for the course **CHP203: Parallel Optimization Techniques** offered by Hugo Taboada and Gabriel Dos Santos as part of the [High Performance Computing & Simulation](https://chps.uvsq.fr/) M.Sc. program at [ISTY/UVSQ](https://www.uvsq.fr/institut-des-sciences-et-techniques-des-yvelines-isty). Its use is reserved for students of the [Paris-Saclay University](https://www.universite-paris-saclay.fr/).

The Spring 2026 session will start on Tuesday, 24 March and end on Tuesday, 28 April.


## Course Information

### Description & objectives

This course provides an overview of common optimization techniques for modern HPC architectures, as well as giving an introduction to supercomputing tools and environments.

By the end of the course, the students are expected to have acquired a thorough understanding of the following concepts:

- Compilers, build systems, and HPC toolchains
- Parallel and distributed programming models
- Parallel and distributed profiling tools
- Performance benchmarking methodology
- Memory and data structure layout optimizations
- CPU microarchitecture optimizations optimizations
- Shared-memory parallelism performance pitfalls & optimizations
- Distributed programming performance pitfalls & optimizations

### Lecture sessions

Tuesday, 13:45 - 17:00 CET, room CN2, Rabelais building, Guyancourt campus.

### Lab sessions

Tuesday, 9:30 - 12:45 CET, room CN2, Rabelais building, Guyancourt campus.

### Examination

This course is evaluated for the 1st Year of Paris-Saclay University's M.Sc. in High Performance Computing & Simulation.

!!! warning

    All lecture and lab sessions are mandatory. Any absence shall be justified to the administration and the course organizers.

**ECTS credits**
: 3 credits (out of 30 semester credits)

**Grades**

| Examination | Grading | Breakdown |
| --- | --- | --- |
| Test | Mid-semester (surprise) test | TBA |
| Project | Report & presentation | TBA |
| Exam | End-semester finals | TBA |
| **Total** | | **100%** |


## Staff Information

| Name | Role | E-mail |
| --- | --- | --- |
| Hugo Taboada | Instructor | [hugo.taboada@cea.fr](mailto:hugo.taboada@cea.fr) |
| Gabriel Dos Santos | Teaching Assistant | [gabriel.dossantos@cea.fr](mailto:gabriel.dossantos@cea.fr) |

Please contact the instructor or TA for any questions regarding the course. E-mails can be sent in either French or English at your convenience.

Be mindful when sending e-mails. If it is your first contact with the instructor or TA, don't forget to present yourself. Try to clearly and concisely express your problem. Detail the steps you have already taken and what you have tried.

!!! note

    For filtering reasons and easier e-mail management from the teaching staff, please make sure that all e-mail subjects you send are in the form: `[M1CHPS-TOP] <your subject>`.

    ***Any e-mail written in an informal manner or without proper syntax will be ignored.***

Additionally, the HPCS Master has a Discord server on which students can reach the TA (handle: `@gabrl`), either by Private Message or through the `#techniques-optimisation-paralleles` channel.

:arrow_right: [**Invite link**](https://discord.gg/8rJ7hvJE)


## Material

### Lectures

Lecture slides are available [here](artifacts/TOP_course_2025.pdf) (last year's slides).

### Labs

Lab material for this course is available on the following GitHub repository: [TOP-26](https://github.com/dssgabriel/TOP-26)

### Resources

**Books**

- [Computer Architecture: A Quantitative Approach](https://www.elsevier.com/books/computer-architecture/hennessy/978-0-12-811905-1) – Hennessy & Patterson
- [Computer Organization and Design](https://www.elsevier.com/books/computer-organization-and-design-risc-v-edition/patterson/978-0-12-820331-6) – Hennessy & Patterson
- [Modern Operating Systems](https://www.pearson.com/en-us/subject-catalog/p/modern-operating-systems/P200000003295) – Tanenbaum
- [Systems Performance](https://www.brendangregg.com/systems-performance-2nd-edition-book.html) – Gregg
- [Introduction to Parallel Computing](https://www.pearson.com/en-us/subject-catalog/p/introduction-to-parallel-computing/P200000003223) – Grama et al.
- [The Art of Multiprocessor Programming](https://www.elsevier.com/books/the-art-of-multiprocessor-programming/herlihy/978-0-12-415950-1) – Herlihy & Shavit
- [Programming Massively Parallel Processors](https://www.elsevier.com/books/programming-massively-parallel-processors/kirk/978-0-323-91231-0) – Kirk & Hwu
- [Parallel Programming in C with MPI and OpenMP](https://www.mheducation.com/highered/product/parallel-programming-c-mpi-openmp-quinn/M9780072822564.html) – Quinn
- [Numerical Linear Algebra](https://epubs.siam.org/doi/book/10.1137/1.9780898719574) – Trefethen & Bau
- [Optimizing Compilers for Modern Architectures](https://www.elsevier.com/books/optimizing-compilers-for-modern-architectures/allen/978-0-08-051345-4) – Allen & Kennedy
- [GPU Gems (3rd edition)](https://developer.nvidia.com/gpugems/gpugems3/part-v-physics-simulation)
- [Hacker's Delight](https://dn710003.ca.archive.org/0/items/random-papers9/Henry%20S.%20Warren%20-%20Hacker%27s%20Delight%20%282nd%20Edition%29-Addison-Wesley%20Professional%20%282012%29.pdf) – H. Warren

**Standards, specifications & documentation**

- [C++ Standard (working draft)](https://eel.is/c++draft/)
- [C++ Reference](https://en.cppreference.com/w/)
- [OpenMP Specification](https://www.openmp.org/specifications/mpi-5.0/mpi50-report.pdf)
- [MPI Standard](https://www.mpi-forum.org/docs/)
- [OpenSHMEM Specification](http://www.openshmem.org/site/sites/default/site_files/OpenSHMEM-1.6.pdf)
- [Kokkos Documentation](https://kokkos.org/kokkos-core-wiki/)

**Papers**

- [What Every Computer Scientist Should Know About Floating-Point Arithmetic](https://www.itu.dk/~sestoft/bachelor/IEEE754_article.pdf) – D. Goldberg
- [What Every Programmer Should Know About Memory](https://people.freebsd.org/~lstewart/articles/cpumemory.pdf) – U. Drepper
- [Scalable Communication Protocols for Dynamic Sparse Data Exchange](https://spcl.ethz.ch/Publications/.pdf/hoefler-dsde-protocols.pdf) - T. Hoefler et al. ([slides](https://spcl.ethz.ch/Publications/.pdf/hoefler-dsde-protocols-slides.pdf))
- [Scientific Benchmarking of Parallel Computing Systems](https://htor.inf.ethz.ch/publications/img/hoefler-scientific-benchmarking.pdf) - T. Hoefler et al. ([slides](https://htor.inf.ethz.ch/publications/img/hoefler-scientific-benchmarking_slides.pdf), [recorded talk](https://youtu.be/HwEpXIWAWTU))
- [Demystifying the Characteristics of High Bandwidth Memory for Real-Time Systems](https://upcommons.upc.edu/server/api/core/bitstreams/b843de39-f32f-4069-8843-48f74c030213/content) - K. Asifuzzaman et al.
- TBA

**Talks**

- [Think Parallel](https://youtu.be/VSDmkwHWpfA)
- [Multidimensional C++ - B. A. Lelbach](https://youtu.be/aFCLmQEkPUw)
- [More Speed & Simplicity: Practical Data-Oriented Design in C++ - V. Romeo](https://youtu.be/zDFSDBcIqhE)
- [The C++ Execution Model](https://youtu.be/6zq5ZmCvldU)
- [How to Tame Packs, `std::tuple`, and the Wily `std::integer_sequence` - A. Alexandrescu](https://youtu.be/X_w_pcPs2Fk)
- [What Every Programmer Should Know about How CPUs Work - M. Godbolt](https://youtu.be/-HNpim5x-IE)
- [`*(char*)0 = 0;` What Does the C++ Programmer Intend With This Code? - J.F. Bastien](https://youtu.be/dFIqNZ8VbRY)

**Websites, blogs & articles**

- [HPC Wiki](https://hpc-wiki.info/hpc/HPC_Wiki)
- [Chips & Cheese](https://chipsandcheese.com/)
- [Daniel Lemire](https://lemire.me/blog/)
- [Matt Godbolt's Advent of Compiler Optimizations (AoCO) 2025](https://xania.org/AoCO2025)
- [Optimizing parallel reductions in CUDA](https://developer.download.nvidia.com/assets/cuda/files/reduction.pdf)
- [Parallel Prefix Sum (Scan) with CUDA](https://developer.nvidia.com/gpugems/gpugems3/part-vi-gpu-computing/chapter-39-parallel-prefix-sum-scan-cuda)
- [Inside NVIDIA GPUs: Anatomy of high performance matmul kernels](https://www.aleksagordic.com/blog/matmul)
- [How to Optimize a CUDA Matmul Kernel for cuBLAS-like Performance: a Worklog](https://siboehm.com/articles/22/CUDA-MMM)
- [Outperforming cuBLAS on H100: a Worklog](https://cudaforfun.substack.com/p/outperforming-cublas-on-h100-a-worklog)
- [Notes About Nvidia GPU Shared Memory Banks](https://feldmann.nyc/blog/smem-microbenchmarks)
- [A (Draft) Taxonomy of SIMD Usage](https://branchfree.org/2024/06/09/a-draft-taxonomy-of-simd-usage/)
- TBA

**Useful tools**

- [Compiler Explorer](https://godbolt.org/)
- [C++ Insights](https://cppinsights.io/)
- [Spack PM](https://spack.io/)
