---
id: hoi0pl51up9fxj0vtn7fmi0
title: File Ownership
desc: ''
updated: 1660669532623
created: 1659854979542
---

- Files have three kinds of permissions:
  - read (**r**)
  - write (**w**)
  - execute (**x**)  

These permissions together constitutes the *mode* of the file.

- These permissions can then be assigned to three different groups of owners/entities:
  - user (**u**)
  - group (**g**)
  - others (**o**)

and `ls -l` command can be used to view the permission and other details of a file
> `ls -l <fileName>`

> *Outputs*  
> `-rwxr--r-x 1 user group 304 Apr 28 10:10 <fileName>`

here,  
$$$\underbrace{\text{-}}_{\small{\texttt{| file type |}}}\underbrace{\text{rwx}}_{\small{\texttt{ user |}}}\underbrace{\text{r- -}}_{\small{\texttt{ group |}}}\underbrace{\text{r-x}}_{\small{\texttt{ others |}}}$$$

</br>

- These utility programs can help configuring the file permissions  
    **chown** : Used to change the user ownership of a file or directory  

    **chgrp** : Used to change the group ownership  

    [[chmod|linux.filesystem.file-operations.file-ownership.chmod]] : Used to change the different permission levels of a file  
