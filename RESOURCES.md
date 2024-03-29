# Cross-lang interop

* ["C Isn’t A Programming Language Anymore", Medium](https://medium.com/@Aaron-007/c-isnt-a-programming-language-anymore-183e432c32db). Est. read. time: 16 mins.
* ["Making Libraries Consumable for Non-C++ Developers - Aaron R Robinson - CppCon 2021"](https://www.youtube.com/watch?v=4r09pv9v1w0). Duration: 58:22.

## ABI

* ["What is an ABI, and Why is Breaking it Bad? - Marshall Clow - CppCon 2020"](https://www.youtube.com/watch?v=7RoTDjLLXJQ). Duration: 1:05:52.

* [CppCon 2019: Louis Dionne “The C++ ABI From the Ground Up”](https://www.youtube.com/watch?v=DZ93lP1I7wU). Duration: 53:34.

* ["How Can Package Managers Handle ABI (In)compatibility in C++? - Todd Gamblin - CppCon 2021"](https://www.youtube.com/watch?v=gWe2K_oCp6A). Duration: 58:28.

### Calling conventions

* ["This Is How Little Birds Secretly Keep Your Code Safe"](https://www.youtube.com/watch?v=z6gdQt8mjn4). Duration: 8:01.

## Object files

* ["CppCon 2017: Michael Spencer “My Little Object File: How Linkers Implement C++”"](https://www.youtube.com/watch?v=a5L66zguFe4). Duration: 47:50.

**Note:** This video explains object files before C++ modules. According to ["C++23 Standard Library Preview - Jeff Garland - CppCon 2021"](https://www.youtube.com/watch?v=ySsqD2e5uRQ), object files will change.

## Static and dynamic libraries

### Dynamically loaded libraries

* [Medium article "Dynamic Linking in Rust’s FFI: Understanding the Essentials"](https://dlcoder.medium.com/dynamic-linking-in-rusts-ffi-understanding-the-essentials-c9e683bebb99)
* ["Dynamically Loaded Libraries Outside the Standard - Zhihao Yuan - CppCon 2021"](https://www.youtube.com/watch?v=-dxCaM4GOqs). Duration: 54:53.

## Debugging information

* [Linux Debuginfo Formats - DWARF, ELF, dwo, dwp - What are They All? - Greg Law - CppCon 2022](https://www.youtube.com/watch?v=l3h7F9za_pc). Duration: 1:02:33.
* ["CppCon 2018: Simon Brand “How C++ Debuggers Work”"](https://www.youtube.com/watch?v=0DDrseUomfU). Duration: 1:00:59.

## Transpilers

* [Github repository of Fable](https://github.com/fable-compiler/fable).

> F# transpiler into Rust, Dart, JavaScript, TypeScript, Python

* [Arxiv paper "Ownership guided C to Rust translation"](https://arxiv.org/abs/2303.10515)

## Compiler backends

### LLVM

#### LLVM vs GIMPLE

* ["How is GCC IR different from LLVM IR?", Stack Overflow](https://stackoverflow.com/questions/40799696/how-is-gcc-ir-different-from-llvm-ir)

#### Intro to LLVM
* ["2019 EuroLLVM Developers’ Meeting: V. Bridgers & F. Piovezan “LLVM IR Tutorial - Phis, GEPs ...”"](https://www.youtube.com/watch?v=m8G_S5LwlTo). Duration: 50:45.

### Cranelift

* [Cranelift compared to LLVM](https://github.com/bytecodealliance/wasmtime/blob/main/cranelift/docs/compare-llvm.md)

## Articles and tooling for languages

## True cross-lang (N x M)

* [GIAC 2021 (Global Internet Architecture Conference) of Alibaba FFI – Exploration of Cross-Language Programming](https://www.alibabacloud.com/blog/an-exploration-of-cross-language-programming_598811)

### Rust

#### Articles & videos (how-to)

* [The Rust FFI Omnibus](http://jakegoulding.com/rust-ffi-omnibus/)

> a collection of examples of using code written in Rust from other languages.

* [Integrating Rust With Android Development](https://blog.devgenius.io/integrating-rust-with-android-development-ef341c2f9cca)

* [SIMD instructions with Rust on Android by Guillaume Endignoux - Rust Zürisee June 2023](https://www.youtube.com/watch?v=x5tK5ET6Q1I)

* [LLVM and Rust, the Dynamics of (Low-Level Virtual Machine)](https://medium.com/@dwulf69/llvm-and-rust-the-dynamics-of-low-level-virtual-machine-a5fe2efb4c50)

#### Corrosion

A tool for integration of Rust into C/C++ project.

* [GitHub page](https://github.com/corrosion-rs/corrosion).

#### Maturin

* ["Calling Rust code from Python"](https://www.youtube.com/watch?v=DpUlfWP_gtg). Duration: 8:22.

#### CPython + PyO3

* ["15. Python Module written in Rust - From Python to Rust"](https://www.youtube.com/watch?v=yqLD22sIYMo&list=PLEIv4NBmh-GsWGE9mY3sF9c5lgh5Z_jLr&index=23). Duration: 20:27.

#### Neon

* [Expose a Rust Library to Other Languages](https://slint-ui.com/blog/expose-rust-library-to-other-languages.html)

#### WAPM

* ["Build Universal Libraries with Rust"](https://www.youtube.com/watch?v=uKlHwko36c4). Duration: 20:58.

### TypeScript

* [Hyperimport - Import c, rust, zig etc. files in TypeScript](https://dev.to/tr1ckydev/hyperimport-import-c-rust-zig-etc-files-in-typescript-1ia5)

# Distribution

* ["Creating and maintaining a conda-forge package"](https://www.youtube.com/watch?v=8s5aj3sjuVE). Duration: 41:30.

* ["Which Python Package Manager Should You Use?", Google Cloud Tech](https://www.youtube.com/watch?v=3J02sec99RM). Duration: 5:05.

**Note:** Both `venv` and `conda` are in use. There's `pyenv` that tries to rule them.

## Dependency management

* [PyConBy 2019: Nikita Grishko, Evolution of dependency management](https://www.youtube.com/watch?v=YErAfIWC0wk). Duration: 35:53.

> An overview of Python tooling for dependency management, together with description of its strengths and weaknesses. The presentation is in Russian but automatically translated subtitles are available.

### Package Managers

* [Stay Together For The Kids - Andrew Kelley - Software You Can Love 2022](https://www.youtube.com/watch?v=stChOsejLEQ). Duration: 26:20.

> On Language Package Managers (LPMs) and System Package Managers (SPMs).

# Note on learning resources

The structure in the resources is meant to eventually emerge.

# On connection of "Related projects, teams, and individual developers" to "Learning resources"

Check the main [README](https://github.com/cross-lang-and-cross-platform/cross-lang-and-cross-platform/blob/main/README.md#on-connection-of-related-projects-teams-and-individual-developers-and-learning-resources).
