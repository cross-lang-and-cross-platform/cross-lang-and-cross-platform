<!-- The README is intentionally written in the design-doc style -->

# What are we trying to build?

We're trying to create tooling that would allow easy generation of [bindings] from code in programming languages whose compilers allow emitting [LLVM]: (1) Rust, (2) ActionScript, (3) Ada, (4) C#, (5) Common Lisp, (6) PicoLisp, (7) Crystal, (8) CUDA, (9) D, (10) Delphi, (11) Dylan, (12) Forth, (13) Fortran, (14) Free Basic, (15) Free Pascal, (16) Graphical G, (17) Halide, (18) Haskell, (19) Java bytecode, (20) Julia, (21) Kotlin, (22) Lua, (23) Objective-C, (24) OpenCL, (25) PostreSQL and PLpgSQL, (26) Ruby, (27) Scala, (28) Swift, (29) XC, (30) Xojo, and (31) Zig.[^1]

## Notes
* The desired properties for the tooling will stem from the intended applications, known challenges, and shortcomings in similar tools and libraries.
* The choice of [LLVM] as the mainstay of the toolings will be justified based on the desired properties.

# Why is such tooling needed?

Such tooling would greatly facilitate **cross-language code reuse** and **cross-platform development**.

This in turn would result in many [person-hours] saved on reimplementations of the same functionality in different programming languages. In addition, the implementations in programming languages like C, C++, Rust, Fortran, and Ada, - according to ["Energy Efficiency across Programming Languages: How Do Energy, Time, and Memory Relate?"] - often have lower latency, higher throughput, thinner memory footprint, and reduced energy consumption. All these runtime characteristics often restrict the choice of programming languages, forcing developers to use not the languages
* that would allow to ship more feature-rich products faster;
* [that the developers love][Most loved, dreaded, and wanted];

but the languages that would provide reasonable runtime characteristics.

According to [Mapped: Energy Consumption Per Capita Around the World], even as small country as Iceland spent 990,097,000 kWh of energy on data centers in 2019. While it's only 5.2% of Iceland's total energy consumption, 65.9% of energy consumption in Iceland was attributed to notoriosly energy-hungry Aluminum smelters whereas less energy-hungry Ferroalloy industry in fact consumed **less** than data centers: 897,846,000 kWh or 4.7% of total energy consumption. Iceland is in a good position.

> Thanks to the country’s abundance of geothermal resources, geothermal and hydropower plants account for more than 99% of Iceland’s electricity generation.

However, renewable supply of energy is limited and even renewable energy is not free. 

|         | Price per kWh                                   |
|---------|-------------------------------------------------|
| Canada  | 0.179 USD                                       |
| Russia  | 0.090 USD                                       |
| Iceland | 0.139 USD (households) / 0.053 USD (businesses) |
| China   | 0.083 USD                                       |
| Brazil  | 0.142 USD                                       |

The table generated with <https://www.tablesgenerator.com/markdown_tables>

**Billions** of dollars are spent worldwide to process data. Such companies as Khan Academy even found it reasonable to rewrite the back-end, which initially was developed in Python, using Golang. As they claimed, the decision was driven by rising bills from cloud service providers. Google invested in the development of Carbon programming language because it wanted safety but interoperability between C++ and Rust is complicated.

## Notes

* The to-be-developed tooling will not compete but coexist and possibly even provide foundation for cross-platform **UI libraries** (such as [Flutter] and [React Native]), i.e. the tooling is intended to be a part of the respective [software ecosystems].
* [Microservices] and [IPC] (inter-process communication) are two other important approaches to cross-language interoperability. They come with considerably greater performance overhead that can be justified in **some** but *not even in the majority of use cases*.

<!-- The claim "but *not even in the majority of use cases*" must be supported with facts -->

# Existing approaches and their issues

Good overview of the prior art is given in the presentation ["Making Libraries Consumable for Non-C++ Developers - Aaron R Robinson - CppCon 2021"]. Duration: 58:22.

# How is the project going to be driven from the financial standpoint?

The team buys the motto of [Rust Foundation],

> "Good software is built by happy, well-supported people".

Once the working group delivers the results that bring undeniable value, the team will consider possible options of getting the financial support for the project. 

# On connection of "Related projects, teams, and individual developers" and "Learning resources"

There will be an inevitable overlap between the two parts of the repository because tools and libraries are developed by people, who create teams, and orgaize projects. However, "Related projects, teams, and individual developers" is meant to be sort of an address book or a telephone directory for potential and actual collaborators, whereas learning resources is supposed to be a place to learn more about cross-language interoperability and cross-platform development.

# Repository navigation

* [History of the project](https://github.com/JohnScience/cross-lang-and-cross-platform/blob/main/HISTORY.md)
* [Our tech stack](https://github.com/cross-lang-and-cross-platform/cross-lang-and-cross-platform/blob/main/OUR_TECH_STACK.md)
* [Sought-after competencies](https://github.com/JohnScience/cross-lang-and-cross-platform/blob/main/SOUGHT_AFTER_COMPETENCIES.md)
* [Learning resources](https://github.com/cross-lang-and-cross-platform/cross-lang-and-cross-platform/blob/main/RESOURCES.md)
* [Related projects, teams, and individual developers](https://github.com/cross-lang-and-cross-platform/cross-lang-and-cross-platform/blob/main/RELATED_TEAMS_AND_PROJECTS.md)
* [Ongoing work](https://github.com/JohnScience/cross-lang-and-cross-platform/blob/main/ONGOING_WORK.md)

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
[person-hours]: https://en.wikipedia.org/wiki/Man-hour
["Energy Efficiency across Programming Languages: How Do Energy, Time, and Memory Relate?"]: https://greenlab.di.uminho.pt/wp-content/uploads/2017/10/sleFinal.pdf
[Most loved, dreaded, and wanted]: https://insights.stackoverflow.com/survey/2021#technology-most-loved-dreaded-and-wanted
[Mapped: Energy Consumption Per Capita Around the World]: https://elements.visualcapitalist.com/energy-consumption-per-capita/
[^1]: https://en.wikipedia.org/wiki/LLVM
