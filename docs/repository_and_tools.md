# Repository and tools

The lab material for this course is available on the following [GitHub repository](https://github.com/dssgabriel/TOP-25).

Most of the software used throught in this course can be easily installed via your Linux's distrubtion package manage (e.g. `apt` on Ubuntu/Debian, `dnf` on RedHat-based, `pacman`/`paru` on Arch, etc.) or using the [Spack Package Manager](https://spack.readthedocs.io/en/latest/index.html).


## Required software

To load Spack-installed software, use the `spack load <PACKAGE>` command.

### Compilers

Compiler | Version | Spack command
--- | --- | ---
GNU Compiler Collection (gcc) | 14.2 | `spack install gcc@14.2.0`
LLVM Clang (clang) | 19.1.7 | `spack install llvm@19.1.7`
Intel oneAPI (icx) | 2025.0.4 | `spack install intel-oneapi-compilers@2025.0.4`

### MPI

Implementation | Version | Spack command
--- | --- | ---
Open MPI | 5.0.6 | `spack install openmpi@5.0.6`
MPICH | 4.2.3 | `spack install mpich@4.2.3`


## Formatting and style

We expect students to format your code according to a `clang-format` spec (one is provided at the root of the lab repo).

To improve your C/C++ code, we suggest you to regularly run tools such as `clang-tidy`, `sonar-lint` or other code linters.

You can also take a look at popular and battle-tested code style guidelines such as:

- [C++ Core Guidelines](https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines)
- [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html)
- [Carbon C++ Style Guide](https://docs.carbon-lang.dev/docs/project/cpp_style_guide.html)
- [MISRA C++](https://misra.org.uk/misra-c-plus-plus/)
- [ANSSI C Rules for C language software development](https://cyber.gouv.fr/en/publications/rules-secure-c-language-software-development)
