# Mastering Rust



# Table of Contents





----



| Parameter        | Value                                    | Note |
| ---------------- | ---------------------------------------- | ---- |
| Official Website | [Click Here](https://www.rust-lang.org/) |      |
|                  |                                          |      |
|                  |                                          |      |



# Rust Binaries



## Rust Version

For check installed rust on your machine, execute this command :

```bash
$ rustc --version
```



## Rust Update 

For update rust to newer version, execute this command : 

```bash
$ rustup update
```



---



# Cargo



## Create Project

To initiate new project execute this command :

```bash
$ cargo new hello
```



---



## Execute Project

Go to hello package and then execute entry point in the project :

```bash
$ cargo run
```

Output :

```
   Compiling hello v0.1.0 (D:\Gitlibertarian\Mastering-Rust\hello)
    Finished dev [unoptimized + debuginfo] target(s) in 1.58s
     Running `target\debug\hello.exe`
Hello, world!
```

To execute in quiet mode add this flags :

```bash
$ cargo run -q
```

Output :

```
Hello, world!
```



---



## Test Project

To test the project create **tests** directory and create file test.rs :

```rust
#[test]
fn works() {
    assert!(true);
}
```

Start testing by execute this command :

```bash
$ cargo test
```

Output :

```
     Running tests\test.rs (target\debug\deps\test-baf0d4e290429966.exe)

running 1 test
test works ... ok

test result: ok. 1 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s
```

