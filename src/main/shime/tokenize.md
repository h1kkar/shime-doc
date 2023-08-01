<div align="center">
    <h1>tokenize</h1>
    <h4>The module processing input arguments.</h4>
</div>

---

### The structure of struct and impl:

```
tokenize
└─ struct Command
   └─ impl Command
      └─ fn start()
```

---

### struct Command

> The structure containing the very first keyword, arguments and subsequent commands.

##### keyword: String

##### args: String

---

### impl Command

#### fn start(c: &String) -> [Command](https://github.com/h1kkar/shime-doc/blob/main/src/main/shime/tokenize.md#struct-command)

> The function that receives commands and displays Command with changed data.

---

<div align="center">
    <h5><a href="https://github.com/h1kkar/shime-doc/blob/main/src/main/shime.md">back</a></h5>
</div>
