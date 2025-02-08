# INTRODUCTION

Learning the intricates of git and github while keeping the knowledge available to anyone interested in understanding how to use it for simple daily activities


# COMMANDS

### Configuration

```shell
> git config --global user.name "Your Name"
> git config --global user.email "Your Email"

```

### Git Status/Add/Commit

- git status
- git add "filename"
- git commit -m "Message"

### Searching for Files

search:
```shell
ls | grep <filename>

```

### ssh-key setup

```shell
ssh-keygen -t rsa -b 4096 -C "email@address" (legacy systems)

ssh-keygen -t ed25519 -C "your_email@example.com" (new systems)

```

### Copying Files on linux/macos

```shell
pbcopy < "filename"

```

### Checking existing ssh key agent running

```shell

eval "$(ssh-agent -s)"

```

### checking if .ssh/config exist

```shell
open ~/.ssh/config
touch ~/.ssh/config #if doesn't exist)

```

Add ssh to agent

```shell
ssh-add --apple-use-keychain ~/.ssh/<keyname>

```

### Adding a Repo from Loal system

```shell
git init
git remote add origin "giturl"
git remote -v
git push -u origin master
```
where "giturl" represents the url to your git repository

# GIT BRANCHING

```shell

git branch # shows the or
git branch -r 

git checkout -b "branchName"
git checkout "branchName" # Switching between branch

git diff <branchnName> #shows changes made

```

# PULL REQUEST

```shell
git merge <branchName> #merge a branch into another branch

git push -u origin <branchName> #push branch to github

```
Pulling down resources from github to update local main repo

```shell
git branch -d <branchName> #To delete a branch
git pull origin main #if you have not set the upstream or
git pull

```
# UNDOING FILES

```shell
git reset <fileName> # Undo commit or stash changes
git reset HEAD 
git reset HEAD~1
git reset <commitID> # resets a specific commit hash
git reset --hard <commitID> #go back and clear all things to its intial file

git log #shows all commits

```

# GIT FORKING
Forking is done on github.com to create a copy of an existing repo from others

# Reference
The following materials/resources were used for studies
- https://www.youtube.com/watch?v=RGOj5yH7evk (freecodecamp)