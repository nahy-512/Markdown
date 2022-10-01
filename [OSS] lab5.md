# [OSS] Lab5
### *Learn Shell Commands 2*
---

### >
>You can redirect output using ">" after a command (e.g.,ls) to create and save the output in a file
### cat
>Command "cat" displays the content of a text file.

![>&cat](https://user-images.githubusercontent.com/101113025/193424639-d0c05edb-4f17-4648-91b7-32226a52e6ba.png)

### >>
>Using ">>" appends output to an existing file (if it already exists), or create and write to a new file if it doesn't exist.
![>>](https://user-images.githubusercontent.com/101113025/193424954-8c90ebc5-98f6-4080-b83b-f089686d1563.png)

### <>
>\* By default, standard input is from keyboard.
\* You can redirect input from a file using "<".
\* You can mix "<" and ">" together in a single line.
![mix](https://user-images.githubusercontent.com/101113025/193425027-e67643e9-2fd4-4093-8c08-3377eb825ffb.png)

### Pipelines "|"
>\* Pipeline feeds output of previous command to input of next command.
\* command1 | command2 | command3 | ...
![pipeline1](https://user-images.githubusercontent.com/101113025/193425488-44a6cdcc-143e-4d95-9725-ae1e32764703.png)
![pipeline2](https://user-images.githubusercontent.com/101113025/193425490-cc6c5183-e33a-4d9f-b6ed-08b31d5a8ebd.png)
\* Press "q" key to exit the screen.
![wc -l](https://user-images.githubusercontent.com/101113025/193425577-f7111a8a-4367-4176-b7ba-765039e38d00.png)

### echo
>Special characters expand its meaning when given to shell commands.
![echo](https://user-images.githubusercontent.com/101113025/193425597-7e7bf7f1-3304-4e4b-a263-7598635cff25.png)  

#### *Tip: Backslash*
>Backslash can be used to ignore line change in command ("enter"), to enter a long command in multi lines

---
## Permissions
* Linux is a multi-user system.
* Files and directories have a permission assigned differently to owner/group/others.
![images](https://images.velog.io/images/estell/post/53d19ba0-ebe3-4ebd-aa75-efe120d4089a/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-02-28%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%2010.15.41.png)
* "chmod" changes permissions.
![images](https://haktuts.github.io/gallery/a836283f9d09a9207660a68a8fbda0ca_681x461.png)

#### *Tip: History*
>Type "history" to see previous command history.
Or, save it to a text file.
![history](https://user-images.githubusercontent.com/101113025/193426250-c1a35298-b921-4a77-afeb-036b0336cbc3.png)
