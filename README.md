# Mastering Git

Project with examples to teach about Git - FJ-87 Caelum Course

### Staging files

Undo last commit, put changes into staging

```bash
$ git reset --soft HEAD^
```

Changing the last commit

```bash
$ git commit --amend -m "New commit message"
```

Changing the last commit without change the message

```bash
$ git commit --amend --no-edit
```
