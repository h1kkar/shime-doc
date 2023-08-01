<div align="center">
    <h1>get</h1>
    <h4>The module that contains the functions displaying this or that information over the input line.</h4>
</div>

---

### The structure of functions:

```
get
├─ fn root()
├─ fn dir()
├─ fn branch()
├─ fn commit()
├─ fn delim()
├─ fn ver()
└─ fn history()
```

---

### fn root()

> The function that prints information about the presence in sudo.

---

### fn dir()

> The function that prints information about the current directory or the name of the git repository in which the user is located.

---

### fn branch()

> The function that prints information about the current guit of the branch if the user is in the repository.

---

### fn commit()

> The function that prints information about the last commit if the user is in the repository.

---

### fn delim()

> The function that prints a separator in the form of a vertical strip, to the next release I will refuse it.

---

### fn ver()

> The function that prints the version of the Cargo project and the version of Rust.

---

### fn history() -> String

> The function that returns the path to the history file (\$HOME/.config/shime/shime_history).


