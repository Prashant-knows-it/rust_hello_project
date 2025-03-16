# Rust Hello World Setup Guide

## Prerequisites

Before getting started, ensure you have the following installed:

1. **Rust & Cargo (Required)**

   - Install via [rustup](https://rustup.rs/):
     ```sh
     rustup-init.exe
     ```
   - On Windows, download and install Rust using [rustup-init.exe](https://win.rustup.rs/).

2. **C++ Build Tools (Required for Windows)**

   - Install [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/) with the following components:
     - MSBuild
     - Windows SDK 11 or whichever version you have
     - C++ CMake tools (optional but recommended)

3. **VS Code (Optional, Recommended)**

   - Download and install [VS Code](https://code.visualstudio.com/).
   - Install the Rust extension (`rust-analyzer`).

---

## Create and Run a Rust Project

To create a new Rust project using Cargo:

```sh
cargo new hello_project
cd hello_project
```

This will create a folder `hello_project` with default files.

To run the project:

```sh
cargo run
```

This will compile and execute `src/main.rs`, printing `Hello, World!` to the console.

---

## Uninstall Rust & Cargo

If you want to remove Rust and Cargo from your system, run:

```sh
rustup self uninstall
```

This will remove Rust, Cargo, and all associated components from your system.

---

### Notes

- **Without Cargo:** You can compile manually using `rustc`:
  ```sh
  rustc src/main.rs -o hello
  ./hello  # Run the binary (./hello.exe on Windows)
  ```
- Cargo simplifies project management by handling dependencies, builds, and execution automatically.

