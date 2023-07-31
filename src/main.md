<div align="center">
    <h1>main.rs</h1>
    <h4>The main shime module</h4>
</div>

---

#### The structure of modules and functions:

```
crate
├─ mod cmd
├─ mod exec
├─ mod shime
└─ fn main()
```

---

#### fn main ()

> The main file that launches `crate::shime::start()`

##### There is no example, because this function simply launches another.

---

#### [mod shime](https://github.com/h1kkar/shime-doc/blob/main/src/main/shime.md)

> The module containing the basic functionality of `shime`.

---

#### [mod exec](https://github.com/h1kkar/shime-doc/blob/main/src/main/exec.md)

> The module containing a function that launches programs.

---

#### [mod cmd](https://github.com/h1kkar/shime-doc/blob/main/src/main/cmd.md)

> The module containing functions for its own commands.
