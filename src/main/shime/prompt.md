<div align="center">
    <h1>prompt</h1>
    <h4>The module, which processes the input and display of important information, for example, the directory, git branch and so on.</h4>
</div>

---

### The structure of modules and functions:

```
prompt
├─ mod get
├─ mod dye
├─ mod dir
├─ mod git
├─ mod cargo
├─ mod sudo
├─ fn exec()
└─ fn line()
```

---

### [mod get](https://github.com/h1kkar/shime-doc/blob/main/src/main/shime/prompt/get.md)

> The module that contains the functions displaying this or that information over the input line.

---

### [mod dye](https://github.com/h1kkar/shime-doc/blob/main/src/main/shime/prompt/dye.md)

> The module that just paints the "arrow before the input".

---

### [mod dir](https://github.com/h1kkar/shime-doc/blob/main/src/main/shime/prompt/dir.md)

> The module that is responsible for how to display the directory or name of the git repository.

---

### [mod git](https://github.com/h1kkar/shime-doc/blob/main/src/main/shime/prompt/git.md)

> The module that displays information about the current branch, the last commite, as well as the presence or absence of non-commited changes in the repository.

---

### [mod cargo](https://github.com/h1kkar/shime-doc/blob/main/src/main/shime/prompt/cargo.md)

> The module that displays information about the project version in the Cargo repository, as well as the current version.

---

### [mod sudo](https://github.com/h1kkar/shime-doc/blob/main/src/main/shime/prompt/sudo.md)

> The module that in sudo displays information about this.

---

### fn exec(c: &str) -> String

> The function that launches a line with useful information and collects data from the keyboard, and also controls the history.

---

### fn line()

> The function that collects important information on the entry field.
