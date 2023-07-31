<div align="center">
    <h1>exec</h1>
    <h4>The module containing a function that launches programs.</h4>
</div>

---

### The structure of functions:

```
fn start()
```

---

### fn start(cmds: &String)

> A function that launches the program according to the argument

##### Example:

```rust
let cmd = "ls".to_string();
start(&cmd);
```

##### Output:

```
LICENSE  readme.md  src
```
