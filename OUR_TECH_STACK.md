# Our current tech stack

<img alt="Rust logo" src="https://upload.wikimedia.org/wikipedia/commons/d/d5/Rust_programming_language_black_logo.svg" width="144" height="144">

* Rust - the default choice for the code that is meant to be executed at run-time or build-time[^1].

<img alt="Python logo" src="https://upload.wikimedia.org/wikipedia/commons/c/c3/Python-logo-notext.svg" width="144" height="144">

* Python 3 - permissible (but not recommended) option if the code you're going to write will be executed only at build-time[^1].

**Language-specific parts can be to a reasonable extent written in the target languages. However, they should not be hard dependencies.**

# Possible additions to the tech stack

<img alt="C++ logo" src="https://upload.wikimedia.org/wikipedia/commons/1/18/ISO_C%2B%2B_Logo.svg" width="144" height="144">

* C++ - if you've mastered it and you're unwilling to [learn Rust](https://github.com/nrc/r4cppp) but want to write the code that is meant to be executed at run-time or build-time.

Ensuring correctness of C++ code is more difficult. It must be well-documented and well-tested. Before addition of C++ to the tech stack, research on use of [`cc`](https://crates.io/crates/cc) and [`bindgen`](https://crates.io/crates/bindgen) must be conducted.

<img alt="C logo" src="https://upload.wikimedia.org/wikipedia/commons/1/18/C_Programming_Language.svg" width="144" height="144">

* Ditto

<!-- HTML doc -->

# Afterword

In the ideal world, the project would be absolutely language-agnostic and any tool or library could be written in any language of choice. However, with increased number of used programming languages comes greater complexity. New contributors will rarely be willing to learn another programming language just to make a contribution. And persistent storage in our computers has finite capacity for interpreters, compilers, and other tools used daily by programmers. If different programming languages did not separate developers, this project would not be born.

According to the weak version of [the principle of linguistic](https://en.wikipedia.org/wiki/Linguistic_relativity), on which research - quoting Wikipedia - "[has produced](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4628110/) positive empirical evidence",

> Linguistic categories and usage \[only\] influence thought and decisions;

or, in another often-quoted version,

> Languages don’t limit our ability to perceive the world or to think about the world, rather, they focus our attention, and thought on specific aspects of the world.

[`cc`]: https://crates.io/crates/cc
[^1]: Build-time in this context refers to the build-time of the toolings. The tools, however, are very likely to be used in the build pipelines, so both performance and correctness there are critical for adoption.
