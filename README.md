# A Wasm3 Runtime Using Rust 

This is a practice project that showcases a Wasm3 Runtime created using Rust. The code uses the **wasm3** library to load the calc.wasm module and calls the module’s exported functions using Bindgen that creates FFI (Foreign Function Interface) wrappers around C/C++ libraries. **wasm3** uses this internally to create Rust wrapper functions and data types around the canonical C library.

## Demo:
```
$ cargo new rust-host
Created binary (application) rust-host package

You can now go into that new directory (rust-host) and open Cargo.toml with your favorite text editor, and add the following dependency:

[dependencies]
wasm3 = {version = "0.1.3", features = ["build-bindgen"]}

$ cargo run

Finished dev [unoptimized + debuginfo] target(s) in 0.02s
Running target/debug/rust-host
Adding 3 and 2: 5
Subtract 10 and 2: 8
Multiply 3 and 2: 6
Divide 10 and 2: 5
```
