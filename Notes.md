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

## Hello world with cargo

`cargo` is a package manager. we can create rust projects with, `cargo new project_name`

This command creates a project given the _project_name_. In the folder, there is an `src` folder with `main.rs`. There is `Cargo.toml` with `Cargo.lock` and also `target` folder.

The _target_ folder is where the build or binary will be.

```sh
# build rust project with cargo
cargo build


# execute binary
./target/debug/project_name
```

With ls:

```sh
# list the content of the project directory
ls

# content of the directory
project_name  build/                     deps/                      examples/                  .fingerprint/              incremental/
```

Another simple way to run this project with cargo, we can do `cargo run`.

```sh
# running cargo run
cargo run

# output
cargo run
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.01s
     Running `target/debug/project_name`
Hello, world!
```

If the content of the `main.rs` file changes, then the output will be:

```sh
   Compiling _1_hello_world_with_cargo v0.1.0 (/home/otumian/Project/console/reading_the_rust_book/_1_hello_world_with_cargo)
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.39s
     Running `target/debug/_1_hello_world_with_cargo`
Hello, world there!
```

We can check if there is no issue of the code we have using, `cargo check`.

```sh
# check rust code
cargo check


# output
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.01s
```
