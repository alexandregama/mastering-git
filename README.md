# Mastering Git

Project with examples to teach about Git - FJ-87 Caelum Course

### Staging files

Show untaged differences since last commit

```bash
$ git status
```

If you add the file in **staged** area, you can not see the modifications using git diff. You need to use the follow:

```bash
$ git diff --staged
```

You can unstage the file

```bash
$ git reset filename HEAD
```

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
