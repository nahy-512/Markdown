# [OSS] Lab6
### *Learn about Git*

## Git config
---
*First-time setup*
```sh
$ git config --global user.name "[YOUR NAME]"
$ git config --global user.email [YOUR EMAIL]
$ git config --global innit.defaultBranch main
```


## git command
---
#### * git init:
*Initializing a Repository in an Existing Directory*
```sh
$ git init
```
-> Create '.git' file in root


#### * git status
*Checking Repository Status*
```sh
$ git status
```

#### * git add
*Adding a new file to be staged (tracked)*
```sh
$ git add .
$ git add [file_name]
```

#### * git rm -cached
*Use when you don't want to commit specfic file*
```sh
$ git rm -cached [file_name]
```

#### * git commit
*Record current version by commit*
```sh
$ git commit -m "[commit message]"
```
***Tip)** `$ git log` to check commit version*

#### * git push
*Upload your files change(commit) to Remote (gitHub)*
```sh
$ git push origin main
$ git push origin [branch_name]
```
***Tip)** `branch`*
```sh
# Check current branch
$ git branch

# Change branch name (master -> main)
$ git branch -m master main

# Create a new branch
$ git branch [new_branch]

# Switch to a new branch
$ git switch [new_branch]
```

#### * .gitignore
*Ignoring a file*
```sh
$ nano .gitignore
```
.gitignore file format
```sh
# ignore all .a files
*.a

#but do track lib.a, even though you're ignoring .a files above
!lib.a

# only ignore the TODO file in the current directory, not subdir/TODO
/TODO

# ignore all files in any directory named build
doc/*.txt

# ignore all .pdf files in the doc/ directory and any of its subdirectories
doc/**/*.pdf
```
*Source: Chacon and Straub, Pro Git(2nd edition)*

***Tip) Steps to remove `.DS_Store`***
What is `.DS_Store` ?
* Abbreviation of *Desktop Service Store*
* Create automatically when access to file within finder of Mac
* It is the file that hasn't nothing to do with project, so doesn't need to upload at gitHub. 

Find all `.DS_Store` in higher directory
```sh
$  find . -name .DS_Store -print0 | xargs -0 git rm -f --ignore-unmatch
```
Add `.DS_Store` to .gitignore (do not upload to gitHub)
```sh
$ echo .DS_Store >> .gitignore
```