<div align="center">
    <h1>cmd.rs</h1>
    <h4>Launching your own teams</h4>
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

> the function of moving along the directors inside your file system

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

---

### fn clr()

### fn exit()
