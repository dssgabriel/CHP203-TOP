# Repository and tools

The lab material for this course is available on the following [GitHub repository](https://github.com/dssgabriel/TOP-25).

Most of the software used throught in this course can be easily installed via your Linux distribution package manager (e.g. `apt` on Ubuntu/Debian, `dnf` on RedHat-like, `pacman`/`paru` on Arch-like, etc.), or using the [Spack Package Manager](https://spack.readthedocs.io/en/latest/index.html).

To load Spack-installed software, use the `spack load <PACKAGE>` command.


## Required software

### CMake

Most of this course material relies on CMake for building the code provided in each exercise.

You can get CMake from [here](https://cmake.org/download/). The prefered version for this course is
[3.31](https://cmake.org/cmake/help/v3.31/release/3.31.html), the minimum required version is
[3.25](https://cmake.org/cmake/help/v3.25/release/3.25.html).

1. Download the binary distribution corresponding to your OS. Prefer the tarball (`.tar.gz`) instead of the shell
script.

2. Unpack the tarball where you have downloaded it:
```sh
tar xzf cmake-3.31.6-linux-x86_64.tar.gz
```

3. Make the CMake executable available in your `PATH`:

    === "Bash"

        ```bash
        printf 'export PATH="%s/cmake-3.31.6-linux-x86_64/bin:$PATH"\n' $(pwd) >> $HOME/.bashrc
        source $HOME/.bashrc
        ```

    === "ZSH"

        ```sh
        printf 'export PATH="%s/cmake-3.31.6-linux-x86_64/bin:$PATH"\n' $(pwd) >> $HOME/.zshrc
        source $HOME/.zshrc
        ```

    === "Fish"

        ```fish
        printf 'set --export --prepend PATH %s/cmake-3.31.6-linux-x86_64/bin\n' $(pwd) >> $XDG_CONFIG_HOME/fish/config.fish
        source $XDG_CONFIG_HOME/fish/config.fish
        ```


### Compilers

Compiler | Version | Spack command
--- | --- | ---
GNU Compiler Collection (gcc) | 14.2 | `spack install gcc@14.2.0`
LLVM Clang (clang) | 20.1.0 | `spack install llvm@19.1.7`
Intel oneAPI (icx) | 2025.1 | `spack install intel-oneapi-compilers@2025.0.4`

### MPI

Implementation | Version | Spack command
--- | --- | ---
Open MPI | 5.0.6 | `spack install openmpi@5.0.6`
MPICH | 4.2.3 | `spack install mpich@4.2.3`


## Formatting and style

We expect students to format their code according to a `clang-format` spec (one is provided at the root of the lab repo). Similarly, CMake files may be formatted using tools such as `gersemi`.

To improve your C/C++ code, we suggest you to regularly run tools such as `clang-tidy`, `sonar-lint` or other code linters that help detect anti-patterns, weird or inefficient coding styles, and suggest ways of writing more idiomatic C/C++.

You can also take a look at popular and battle-tested code style guidelines such as:

- [C++ Core Guidelines](https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines)
- [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html)
- [Carbon C++ Style Guide](https://docs.carbon-lang.dev/docs/project/cpp_style_guide.html)
- [MISRA C++](https://misra.org.uk/misra-c-plus-plus/)
- [ANSSI C Rules for C language software development](https://cyber.gouv.fr/en/publications/rules-secure-c-language-software-development)
