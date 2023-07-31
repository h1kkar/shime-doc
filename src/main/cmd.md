<div align="center">
    <h1>cmd.rs</h1>
    <h4>Launching your own commands</h4>
</div>

---

### The structure of use

> crate::shime
> ├─ tokenize::\*
> 
> └─ func
>      ├─dir
>      │  ├─ self
>      │  └─ go
>      └─ say,
> 
> [ansi_colors::\*](https://docs.rs/ansi-colors/0.3.0/ansi_colors/)

---

### The structure of functions:

> cmd
> 
> ├─ [fn cd()](https://github.com/h1kkar/shime-doc/blob/main/src/main/cmd.md#fn-cd)
> 
> ├─ [fn clr()](https://github.com/h1kkar/shime-doc/blob/main/src/main/cmd.md#fn-clr)
> 
> └─ [fn exit()](https://github.com/h1kkar/shime-doc/blob/main/src/main/cmd.md#fn-exit)

---

### fn cd(cmds: Command)

> A function of moving along the directors inside your file system

##### Example:

```rust
println!("{}", env::current_dir().unwrap());
cd(Command { keyword: "cd".to_string(), args: "project/shime" })
println!("{}", env::current_dir().unwrap());
cd(Command { keyword: "cd".to_string(), args: ".." })
println!("{}", env::current_dir().unwrap());
cd(Command { keyword: "cd".to_string(), args: "" })
```

##### Output:

```
you moved to the project/shime dir
you moved to the project dir
you moved to the home dir
```

Dependencies:

> [ansi_colors]([ansi_colors - Rust](https://docs.rs/ansi-colors/0.3.0/ansi_colors/))

---

### fn clr()

> A function that displays a set of colors.
> I need it to select colors (in the future it will change the name or completely disappear as unnecessary)

Dependencies:

> [ansi_colors]([ansi_colors - Rust](https://docs.rs/ansi-colors/0.3.0/ansi_colors/))

---

### fn exit()

> A function that comes out of the terminal and prints goodbye-message
