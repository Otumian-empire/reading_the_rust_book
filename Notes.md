# Notes on rust

## Installation

- Just follow [this instructions](https://doc.rust-lang.org/book/title-page.html) and you'd be good.

## Hello world in rust

```rust
// file name = main.rs
fn main() {
    println1("Hello world!");
}
```

> Compile and Execute

```sh

# use rustc to compile
rustc main.rs

# then run
./main
```

We could use [cargo](https://doc.rust-lang.org/cargo/) to create a rust project.

`cargo --version` should return an output like _cargo 1.80.1 (376290515 2024-07-16)_. If that is not the case, go to the installation part.
