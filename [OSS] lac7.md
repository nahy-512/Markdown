
#### * git rm
*Use "git rm" instead of "rm" for removing a file from both file system and repository*
```sh
$ git rm [file_name]
```

#### * git rm -cached
*Use when you don't want to commit specific file.*
*You can keep files in the system, but untrack them.*
```sh
$ git rm -cached [file_name]
```

#### * git mv
*Use to rename files*
```sh
$ git mv [file_name] [new_name]
```


#### * git log
*Use to check all commit history*
```sh
$ git log
```

#### * git restore
*Unstaging a staged file*
```sh
$ git restore --staged [file_name]
```

#### * git rm -cached
*Use when you don't want to commit specfic file*
```sh
$ git rm -cached [file_name]
```

## Git Push to Remote Repository

```sh
$ git remotre add origin [github_repo_link]
$ git remote -v
$ git push -u origin main
