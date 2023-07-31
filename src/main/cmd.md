<div align="center">
    <h1>cmd</h1>
    <h4>The module containing functions for its own commands.</h4>
</div>

---

### The structure of functions:

```
cmd
├─ fn cd()
├─ fn clr()
└─ fn exit()
```

---

### fn cd(cmds: Command)

> A function of moving along the directors inside your file system

##### Example:

```rust
println!("{}", env::current_dir().unwrap());
cd(Command { keyword: "cd".to_string(), args: "project/shime" });
println!("{}", env::current_dir().unwrap());
cd(Command { keyword: "cd".to_string(), args: ".." });
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

> A function that displays a set of colors.
> I need it to select colors (in the future it will change the name or completely disappear as unnecessary)

---

### fn exit()

> A function that comes out of the terminal and prints goodbye-message
