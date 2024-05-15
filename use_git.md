# overview
1. `git add filename`
2. `git commit -m "your message"`
    - commit can be executed only when at least one add/rm has been executed. 
3. `git push`

others:

- `git status`
- `git log` to view commit log
- `git rm` remove the file in staging area **and directory**
- `git rm --cached` remove the file in staging area
- `git restore <file>` to discard changes since last add for both Dir and Sta.
- `git restore --staged <file>` to discard changes since last commit for staging area.

1. Sta=staging area
2. Dir=directory


# set your name and email

instruction to view your config

```shell
git config --list
git config -l
git config --global -l
```

## set for all repository

`git config --global user.name "Mona Lisa"`
`git config --global user.email "YOUR_EMAIL"`

## set for current local repository

`git config user.name "Mona Lisa"`
`git config user.email "YOUR_EMAIL"`

# .gitignore
- creat manually
- using instruction `touch .gitignore`

# branch
- `git branch` to view all branches.
- `git checkout -b <new branch name>` to create a new branch.
- `git checkout <branch name>` to switch to another branch.
- `git branch -d <branch name>` to delete a branch.

# addition
- `git remote -v` '-v' represents verbose.
