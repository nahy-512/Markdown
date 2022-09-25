# [OSS] Lab4
### *Learn Shell Commands*

---
### pwd
> show the current path in a hirarchical derectory
### ls
> list files and directories
### cd
> change directory
> \* 같은 알파벳으로 시작하는 폴더가 있다면 Tab으로 폴더 이동 불가

![pwd](https://user-images.githubusercontent.com/101113025/192091012-93c07186-902c-4cb3-a352-17c2fb637adb.png)

argument  | description
------------- | -------------
   /          |        root
   .          |   current directory
   ..         |  upper-level-directory
   ~          |  home of current user


![pwd](https://user-images.githubusercontent.com/101113025/192101424-1ede6d4a-b91a-4395-bd7b-d7fe30b6e631.png)

### -l
> show detail information (long format)
### -lh
> same as above, but size in units


### Tip
    * Autocompletion: Press "tab" key
    * Past commands: Press "up arrow" key
    * Shell command: $ clear
    * Help command: $ help/man
    * Exiting terminal: $ exit
    
## Manipulation
---
_***Warning***: These commands may ***delete*** or ***overwrite*** your files and directories._
*Make sure to backup your important contents.

### cp
> copy files and directories
![cp](https://user-images.githubusercontent.com/101113025/192102101-7d5ec9c9-56b0-470a-867a-eb1538007fce.png)


Command | Results
---------------- | -------------
cp file1 file2 | Copies the contents of file1 into file2. If file2 does not exist, it created.
cp -i file1 file2 | Like above however, since the "-i" (interactive) option is specified, if file2 exists, the user is prompted before it is overwritten with the contents of file1.
cp file1 dir1 | Copy the contents of file1 inside of diretory dir1.
cp -R dir1 dir2 | Copy the contents of the diretory dir1. If directory dir2 does not exist, it is created.

### mv
> move files and directoriesor rename them
![mv](https://user-images.githubusercontent.com/101113025/192102325-76eb5c6a-0857-45b1-a9b8-82a44303d0b5.png)

Command | Resualt
--------- | ---------
mv file1 file2 | If file2 does not exist, then file1 is renamed file2. ***if file2 exists, its contents are silently replaced with the contents of file1.***
mv -i file1 file2 | Like above however, since the "-i" (interactive) option is specified, if file2 exists, the user is pormpted before it is overwritten with the contents of file1.
mv file1 file2 dir1 | The files file1 and file2 are moved to directory dir1. If dir1 does not exist, ***mv*** will exit with an error.
mv dir1 dir2 | If dir2 does not exist, then dir1 is renamed dir2. If dir2 exists, the directory dir1 is moved within directory dir2.

### rm
> delete files and directories ***permantely*** and ***irreversevely***
![rm](https://user-images.githubusercontent.com/101113025/192102543-56d40032-2604-41d6-9e0a-ca87f071acf8.png)

Command | Results
------- | -------
rm file1 file2 | Delete file1 and file2.
rm -i file1 file2 | Like above however ,since the "-i" (interactive) option is specified, the user is prompted before each file is deleted.
rm -r dir1 dir2 | Directories dir1 and dir2 are deleted along with all of their contents.

### mkdir
> make a new directory
![mkdir](https://user-images.githubusercontent.com/101113025/192102644-d00f07c4-802c-4054-bef8-c056f7ede7f0.png)

[Source](https://linuxcommand.org/lc3_lts0050.php)

---
## Manipulation: Wildcards

Pattern | Matches
------- | -------
* | All filenames
g* | All filenames that begin with the character "g"
b*.txt | All filenames that begin with the character "b" and end with the characters ".txt"
Data??? | Any filename that begins with the character "Data" followed by exactly 3 more characters

![wildcards](https://user-images.githubusercontent.com/101113025/192155770-64f0a0cd-42b2-40f0-b2ca-78a6413e1176.png)