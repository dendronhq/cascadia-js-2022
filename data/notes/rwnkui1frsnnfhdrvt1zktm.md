
@polesdesfetes

Staff engineer at Data Dog.

V8 Engine
- Takes JS as input and executes it
- Createed by Google, open source, C++
    - https://chromium.googlesource.com/v8/v8.git
- [good resource](https://v8.dev)
- `document` is not defined in V8
- Doesn't just interpret JS
    - Parse to AST
    - Ignition: bytecode generation
    - Sparkplug: fast codegen
    - Turbofan: optimized codegen
    - reminder you can define numbers as `1_000_000` in js
        - [underscore in numbers](https://www.javascripttutorial.net/es-next/javascript-numeric-separator/)
    - objects have a Map, a hidden class.
    - what is % in fromnt of functions?  It's "Native syntaxes". `console.log(%MaxSmi())`
    - You can set V8 flages with node using `require('v8').setFlags (?) ('--flag')`
    - Native syntax: undocumented V8 APIs.
    - Benchmark JS for testing optimizations... optimizations DO matter, up to 2x faster for a simple add function.
    - `V8OptimizationStoatus()` to get the status of optimization
    - How do debuggers work?
        - Chrome Debug Protocol
            - Has a Heap profiler and CPU profiler
                - CPU profiling is done with polling, similar to the `top` program (?)
    - See the Torque language which compiles directly into v8 bytecode. [torque](https://v8.dev/docs/torque)