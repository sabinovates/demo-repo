# INTRODUCTION

Learning the intricates of git and github while keeping the knowledge available to anyone interested in understanding how to use it for simple daily activities


# COMMANDS

### Configuration

```shell
> git config --global user.name "Your Name"
> git config --global user.email "Your Email"

```

### Git Status/Add/Commit
ß
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

# CODE SNIPPETS