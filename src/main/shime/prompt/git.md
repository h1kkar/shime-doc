<div align="center">
    <h1>git</h1>
    <h4>The module that displays information about the current branch, the last commite, as well as the presence or absence of non-commited changes in the repository.</h4>

</div>

---

### The structure of struct, modules and functions:

```
git
├─ struct Conf
│  ├─ branch
│  ├─ dirty
│  └─ lastcommit
├─ mod get
├─ mod alt_conf
└─ fn config()
```

---

### struct Conf

> A structure that stores the name of the git branch, the status of changes and the hash of the last commit.

##### branch: String

##### dirty: bool

##### lastcommit: String

---

### [mod get](https://github.com/h1kkar/shime-doc/blob/main/src/main/shime/prompt/git/get.md)

> The module that displays information about the git repository.

---

### [mod alt_conf](https://github.com/h1kkar/shime-doc/blob/main/src/main/shime/prompt/git/alt_conf.md)

> The module that, in the absence of some data in Conf, is looking for a way to fill in passes.

---

### fn config() -> [Conf](https://github.com/h1kkar/shime-doc/blob/main/src/main/shime/prompt/git.md#struct-conf)

> The function that displays information contained in the Conf struct.
