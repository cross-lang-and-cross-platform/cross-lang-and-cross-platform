<!-- The README is intentionally written in the design-doc style -->

# What are we trying to build?

We're trying to create tooling that would allow easy generation of [bindings] from code in programming languages whose compilers allow emitting [LLVM]: (1) Rust, (2) ActionScript, (3) Ada, (4) C#, (5) Common Lisp, (6) PicoLisp, (7) Crystal, (8) CUDA, (9) D, (10) Delphi, (11) Dylan, (12) Forth, (13) Fortran, (14) Free Basic, (15) Free Pascal, (16) Graphical G, (17) Halide, (18) Haskell, (19) Java bytecode, (20) Julia, (21) Kotlin, (22) Lua, (23) Objective-C, (24) OpenCL, (25) PostreSQL and PLpgSQL, (26) Ruby, (27) Scala, (28) Swift, (29) XC, (30) Xojo, and (31) Zig.[^1]

## Notes
* The desired properties for the tooling will stem from the intended applications, known challenges, and shortcomings in similar tools and libraries.
* The choice of [LLVM] as the mainstay of the toolings will be justified based on the desired properties.

# Why is such tooling needed?

Such tooling would greatly facilitate **cross-language code reuse** and **cross-platform development**.

## Notes

* The to-be-developed tooling will not compete but coexist and possibly even provide foundation for cross-platform **UI libraries** (such as [Flutter] and [React Native]), i.e. the tooling is intended to be a part of the respective [software ecosystems].
* [Microservices] and [IPC] (inter-process communication) are two other important approaches to cross-language interoperability. They come with considerably greater performance overhead that can be justified in **some** but *not even in the majority of use cases*.

<!-- The claim "but *not even in the majority of use cases*" must be supported with facts -->

# Existing approaches and their issues

Good overview of the prior art is given in the presentation ["Making Libraries Consumable for Non-C++ Developers - Aaron R Robinson - CppCon 2021"]. Duration: 58:22.

# Are there any teams or individual developers working on similar problems?

Almost surely, yes. The are plans to create a list of teams and individual developers working on related problems and make the interaction with them as transparent and easy as possible.

# How is the project going to be driven from the financial standpoint?

The team buys the motto of [Rust Foundation],

> "Good software is built by happy, well-supported people".

Once the working group delivers the results that bring undeniable value, the team will consider possible options of getting the financial support for the project. 

# Repository navigation

* [History of the project](https://github.com/JohnScience/cross-lang-and-cross-platform/blob/main/HISTORY.md)
* [Ongoing work](https://github.com/JohnScience/cross-lang-and-cross-platform/blob/main/ONGOING_WORK.md)
* [Our tech stack](https://github.com/cross-lang-and-cross-platform/cross-lang-and-cross-platform/blob/main/OUR_TECH_STACK.md)
* [Sought-after competencies](https://github.com/JohnScience/cross-lang-and-cross-platform/blob/main/SOUGHT_AFTER_COMPETENCIES.md)

# Communications

* Discord server of the working group: https://discord.gg/8xUXjshS4m

[bindings]: https://en.wikipedia.org/wiki/Language_binding
[LLVM]: https://llvm.org/docs/LangRef.html#abstract
["Making Libraries Consumable for Non-C++ Developers - Aaron R Robinson - CppCon 2021"]: https://www.youtube.com/watch?v=4r09pv9v1w0
[Flutter]: https://en.wikipedia.org/wiki/Flutter_(software)
[React Native]: https://en.wikipedia.org/wiki/React_Native
[software ecosystems]: https://en.wikipedia.org/wiki/Software_ecosystem
[Rust Foundation]: https://foundation.rust-lang.org/
[Microservices]: https://towardsdatascience.com/microservice-architecture-a-brief-overview-and-why-you-should-use-it-in-your-next-project-a17b6e19adfd
[IPC]: https://en.wikipedia.org/wiki/Inter-process_communication
[^1]: https://en.wikipedia.org/wiki/LLVM
