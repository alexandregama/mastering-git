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

You can unstage the file. **HEAD** refer to last commit

```bash
$ git reset HEAD filename
```

Undo last commit, put changes into staging. This command moves the commit before **HEAD**

```bash
$ git reset --soft HEAD^
```

Changing the last commit. This message will override the previous commit message

```bash
$ git commit --amend -m "New commit message"
```

Changing the last commit without change the message

```bash
$ git commit --amend --no-edit
```

Adding changes from all tracked files

```bash
$ git commit -a -m "New commit message"
```

If all that commit are wrong, you can reset the changes into staged area and then checkout all your modifications. Undo last commit and all changes.

```bash
$ git reset --hard HEAD^
```

You can undo the last 2 commit and all changes

```bash
$ git reset --hard HEAD^^
```
