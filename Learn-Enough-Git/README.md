# Learn Enough Git to Be Dangerous

This is a sample repository for the [_Learn Enough Git to Be Dangerous_](https://www.learnenough.com/git-tutorial) tutorial.

## Commands

### Initialize a new Git repository

```bash
git init
```

### Check the status of the repository

```bash
git status
```

### Add a file to the staging area

```bash
git add .
# or
git add <filename>
```

### Commit changes

```bash
git commit -m "Commit message"
```

#### View the commit log

```bash
git log
```

#### Change the last commit message

```bash
git commit --amend
```

#### Add and commit changes in one step

```bash
git commit -am "Commit message"
```

### View the changes made to the files

```bash
git diff
```

### First push to GitHub

```bash
git remote add origin <repository-url>
git push -u origin master
```

The `-u` option to git push sets GitHub as the upstream repository, which means we’ll be able to download any changes automatically when we run `git pull`.
