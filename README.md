# runas

[![Build Status](https://github.com/mitsuhiko/rust-runas/workflows/Tests/badge.svg?branch=master)](https://github.com/mitsuhiko/rust-runas/actions?query=workflow%3ATests)
[![Crates.io](https://img.shields.io/crates/d/rust-runas.svg)](https://crates.io/crates/rust-runas)
[![License](https://img.shields.io/github/license/mitsuhiko/rust-runas)](https://github.com/mitsuhiko/rust-runas/blob/master/LICENSE)
[![rustc 1.48.0](https://img.shields.io/badge/rust-1.48%2B-orange.svg)](https://img.shields.io/badge/rust-1.48%2B-orange.svg)
[![Documentation](https://docs.rs/rust-runas/badge.svg)](https://docs.rs/rust-runas)

A simple Rust library that can execute commands as root.

```rust
use runas::Command;

let status = Command::new("rm")
    .arg("/usr/local/my-app")
    .status()
    .unwrap();
```

## License and Links

* [Documentation](https://docs.rs/runas/)
* [Issue Tracker](https://github.com/mitsuhiko/rust-runas/issues)
* [Examples](https://github.com/mitsuhiko/rust-runas/tree/master/examples)
* License: [BSD-3-Clause](https://github.com/mitsuhiko/rust-runas/blob/main/LICENSE)
