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

## syntax
```shell
filename   # ignore a file
directory/ # ignore a directory
*.cpp      # * represents any number of characters or no character.
?          # ? represents a character.
[abc]      # represents a character of a,b,c.
!filename  # do not ignore this file. This sentence overrides others.
```

# branch
- `git branch` to view all branches.
- `git checkout -b <new branch name>` to create a new branch.
- `git checkout <branch name>` to switch to another branch.
- `git branch -d <branch name>` to delete a branch.

# reset
roll back to last commit:
`git reset --hard HEAD` or `git reset --hard HEAD~0`

Roll back to the second to last commit:
`git reset --hard HEAD^` or `git reset --hard HEAD~1`

Roll back using hash(`git reflog` or `git log`):
`git reset --hard <commit-hash>`


- `git reset --soft` to preserve changes for both Dir, Sta.
- `git reset --mixed` to preserve changes for Dir but empty Sta.

# addition
- `git remote -v` '-v' represents verbose.
