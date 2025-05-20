Here’s a short explanation of **compiler** and **interpreter** with examples:

### **Compiler**:

* Translates the entire source code into machine code **before** execution.
* Faster execution after compilation.
* Example: **C** – Code is compiled using `gcc` before running.

### **Interpreter**:

* Translates and runs the code **line by line** at runtime.
* Slower but easier for debugging.
* Example: **Python** – Code runs directly using the Python interpreter (`python script.py`).

**Summary**:
Compiler = Translate all → Then run
Interpreter = Translate and run line-by-line

----

Here's a simple table categorizing some common programming languages based on whether they are typically **compiled** or **interpreted**:

| Language   | Type                   | Notes                                                                 |
| ---------- | ---------------------- | --------------------------------------------------------------------- |
| C          | Compiled               | Uses compilers like `gcc`; fast execution after compilation.          |
| C++        | Compiled               | Similar to C; often compiled with `g++`.                              |
| Java       | Compiled + Interpreted | Compiled to bytecode (via `javac`), then run on JVM (interpreted).    |
| Python     | Interpreted            | Runs line-by-line using the Python interpreter.                       |
| JavaScript | Interpreted            | Executed by web browsers, but now also optimized with JIT techniques. |
| Ruby       | Interpreted            | Runs via the Ruby interpreter.                                        |
| Go         | Compiled               | Compiled to machine code with `go build`.                             |
| Swift      | Compiled               | Compiled with Apple’s LLVM-based toolchain.                           |
| PHP        | Interpreted            | Interpreted by a web server like Apache with PHP module.              |
| Rust       | Compiled               | Compiles to efficient machine code using `rustc`.                     |

> 🔹 **Note**: Some modern languages (like JavaScript and Java) use **JIT (Just-In-Time)** compilation, which combines both interpreted and compiled approaches for better performance.
