<div align="center">
    <h1>dir</h1>
    <h4>The module in which crate::cmd::cd() needs directly needs.</h4>
</div>

---

### The structure of functions:

```
dir
├─ fn home_dir()
├─ fn go()
├─ fn back()
├─ fn next()
├─ fn absolute_path()
└─ fn go_home()
```

---

### fn home_dir () -> String

> The function returning the way to the home directory.

##### Example:

```rust
println!("home dir: {}", home_dir());
```

##### Output:

```
home dir: /home/user
```

---

### fn go (path: &String)

> The function that moves you to the directories and tells you about it.

##### Example:

```rust
let path = "project".to_string();
go(&path);
let path = "..".to_string();
go(&path);
let path = "/".to_string();
go(&path);
```

##### Output:

```
you moved to the project dir
you moved to the home dir
you moved to the / dir
```

---

### fn back() -> Result\<bool, io::Error\>

> The function that, when calling, goes to the directory back and returns a bully or error (due to mechanics of the transition to directory).

##### Example:

```rust
println!("before: {}", env::current_dir().unwrap());
let _ = back();
println!("after: {}", env::current_dir().unwrap());
```

##### Output:

```
before: /home/user/project
after: /home/user
```

---

### fn next(path: &Vec\<String\>) -> Result\<bool, io:Error>

> The function that moves forward along the directors depending on the path that was set in the form of a String array.

##### Example:

```rust
println!("before: {}", env::current_dir().unwrap());
let path: Vec<String> = vec!["project".to_string];
let _ = next(&path);
println!("after: {}", env::current_dir().unwrap());
```

##### Output:

```
before: /home/user
after: /home/user/project
```

---

### fn absolute_path(path: &Vec\<String\>) -> Result\<Option\<String\>, io::Error\>

> The function, which is essentially a copy of the fn next(), but it takes the absolute path to the directory as an argument and returns Ok(None), but the unchifier is still ignored.

##### Example:

```rust
println!("before: {}", env::current_dir().unwrap());
let path: Vec<String> = vec!["/".to_string(), "home/".to_string(), "user/".to_string(), "project".to_string(];
let _ = absolute_path(&path);
println!("after: {}", env::current_dir().unwrap());
```

##### Output:

```
before: /home/user
after: /home/user/project
```

---

### fn go_home() -> Result\<Option\<String\>, io:Error\>

> The function that changes the current directory for home.

##### Example:

```rust
println!("before: {}", env::current_dir().unwrap());
let _ = go_home();
println!("after: {}", env::current_dir().unwrap());
```

##### Output:

```
before: /home/user/project
after: /home/user
```

---

<div align="center">
    <h5><a href="">back</a></h5>
</div>
