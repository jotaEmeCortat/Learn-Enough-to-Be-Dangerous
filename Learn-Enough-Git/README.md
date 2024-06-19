# Learn Enough Git to Be Dangerous

This is a sample repository for the [_Learn Enough Git to Be Dangerous_](https://www.learnenough.com/git-tutorial) tutorial.


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

### Add remote repo

```bash
git remote add origin <repository-url>
git push -u origin master
```

The `-u` option to git push sets GitHub as the upstream repository, which means we’ll be able to download any changes automatically when we run `git pull`.

### Push changes to GitHub

```bash
git push
```

## .gitignore

The `.gitignore` file is used to specify files that should be ignored by Git.

```shell
#project/.gitignore
# Ignore .DS_Store files
.DS_Store
```

### wildcards

```shell
# Ignore all .a files
*.a

# but do track lib.a, even though you're ignoring .a files above
!lib.a

# Ignore all files in the build/ directory
build/

# Ignore doc/notes.txt, but not doc/server/arch.txt
doc/*.txt

# Ignore all .pdf files in the doc/ directory
doc/**/*.pdf

# Ignore all files in any directory named temp
**/temp/
```

## Git Branches

### Create a new branch

```bash
git checkout -b <branch-name>
```

### List all branches

```bash
git branch
```
