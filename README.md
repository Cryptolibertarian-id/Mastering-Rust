# Mastering Rust



# Table of Contents





----



| Parameter        | Value                                    | Note |
| ---------------- | ---------------------------------------- | ---- |
| Official Website | [Click Here](https://www.rust-lang.org/) |      |
|                  |                                          |      |
|                  |                                          |      |



# Rust Language



## Rust is Compiled Language



## Rust is Safe Language



### Type Checking

Every time we create a variable we must first determine the data type to be used. This protects developers from a bunch of common bugs and security flaws in the code we write.



---



### Static Typed

Rust is a statically typed language, mean  a variable created with a certain data type cannot be used on other data types. Look at the code below:

```rust
let data:i32 = 15;
data = "Hello World!";
```

The advantage of static typing is that the compilation results produce code that can be executed quickly, because the compiler knows what data types are used so that it is able to produce optimized machine code.

Optimization provides added value such as speed and lighter memory usage in the application software produced.



---



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



# Introduction to Rust



## Comment

Example of single line and multi-line comment :

```rust
//this is single line comment

/* This is a
Multi-line comment
*/
```

