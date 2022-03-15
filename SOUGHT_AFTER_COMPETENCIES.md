# Sought-after competencies

Creating tooling that would allow easy generation of [bindings] from code in programming languages whose compilers allow emitting [LLVM] is a complex task requiring a diverse set of competencies.

* [LLVM Compiler Infrastructure]
  - [LLVM human-readable language][LLVM] - **necessary**
  - Tool usage - **extremely useful**
* [Parsing]
  - Parsing combinators
    + In general - **useful**
    + [`nom`] - **necessary**
* [SWIG]
  - Tool usage - **extremely useful**
  - Source code - **potentially useful**
* [LLVM-CBE]
  - Tool usage - **potentially useful**
  - Source code - **extremely useful**
* [Language-specific FFI (foreign function interface)][FFI]
  - Python
    + In general - **useful**
    + [CFFI](https://cffi.readthedocs.io/en/latest/) - **extremely useful**
  - Java
    + In general - **extremely useful**
    + [JNI](https://en.wikipedia.org/wiki/Java_Native_Interface) - **potentially useful**
    + [JNA](https://github.com/java-native-access/jna) - **potentially useful**
  - Kotlin
    + In general - **potentially useful**
    + [cinterop](https://kotlinlang.org/docs/native-c-interop.html)
      * Tool usage - **extremely useful**
      * Source code - **extremely useful**
      * `.def` files - **extremely useful**
  - Swift
    + In general - **extremely useful**
  - Dart
    + In general - **potentially useful**
    + [dart:ffi](https://dart.dev/guides/libraries/c-interop) - **extremely useful**
  - JavaScript
    + In general - **extremely useful**
    + Node.js
      * In general - **useful**
      * [C++ addons](https://nodejs.org/api/addons.html#c-addons) - **extremely useful**
    + WebAssembly - **extremely useful**
  - Other programming languages are under consideration
* Packages and package-management ecosystem(-s)
  - Python
    + In general - **potentially useful**
    + [pip](https://en.wikipedia.org/wiki/Pip_(package_manager)) - **extremely useful**
  - Java
    + In general - **extremely useful**
    + [Maven](https://maven.apache.org/) - **extremely useful**
    + [Gradle] - **extremely useful**
  - Kotlin
    + In general - **extremely useful**
    + [Gradle] - **extremely useful**
  - Swift
    + In general - **potentially useful**
    + [Swift Package Manager](https://www.swift.org/package-manager/) - **extremely useful**
  - Dart
    + In general - **potentially useful**
    + [Pub](https://pub.dev/) - **extremely useful**
  - JavaScript
    + In general - **extremely useful**
    + [npm](https://www.npmjs.com/) - **extremely useful**
    + [yarn](https://en.wikipedia.org/wiki/Yarn_(package_manager)) - **extremely useful**
* [Compiler Theory] - **potentially useful**
* [Type Theory] - **potentially useful**

[bindings]: https://en.wikipedia.org/wiki/Language_binding
[LLVM]: https://llvm.org/docs/LangRef.html#abstract
[LLVM Compiler Infrastructure]: https://llvm.org/
[Parsing]: https://en.wikipedia.org/wiki/Parsing
[`nom`]: https://crates.io/crates/nom
[LLVM-CBE]: https://github.com/JuliaComputingOSS/llvm-cbe
[Compiler Theory]: https://en.wikipedia.org/wiki/Compiler#Compiler_construction
[Type Theory]: https://en.wikipedia.org/wiki/Type_theory
[SWIG]: http://www.swig.org/
[FFI]: https://en.wikipedia.org/wiki/Foreign_function_interface
[Gradle]: https://en.wikipedia.org/wiki/Gradle
