---
id: b9tg7hy8dxoef2rqpefdadl
title: chmod
desc: ''
updated: 1660669115502
created: 1660312132481
---

**chmod** is used to change the file *mode* bits of each given file, which can be either a symbolic representation of changes to make, or an octal number representing the bit pattern for the new *mode* bits.

### Symbolic mode

- The format is

    > [ugoa...] [-+=] [perms...]

where, *perms* is either zero or more letters from the set [**r w x X s t**]. Multiple symbolic modes can be given, separated by commas.  

- The letters [**r w x X s t**] selects file *mode* bits for the affected entity:  
read (**r**), write (**w**), execute (or search for directories) (**x**), execute/search only if the file is a directory or already has execute permission for some user (**X**), set user or group ID on execution (**s**), restricted deletion flag  or sticky bit (**t**).

> **eg:**  
> **$** `ls -l <someFile>`  
> -rw-rw-r-- 1 user group 304 Apr 28 10:10 <someFile\>  
>
> **$** `chmod uo+x,g-w <someFile>`  
> **$** `ls -l <someFile>`  
> -rwxr--r-x 1 user group 304 Apr 28 10:10 <someFile\>

If none of these are given, the effect is as if all (**a**) were given, but bits that are set in the umask are not affected.

### Octal mode

- The permissions for each entity can also be represented numerically. This is done by assigning a value to each permission.  

 Permission | Value
 :---|:---:|
 Read | 4
 Write | 2
 Execute | 1

 Using these values, the permissions assigned to User, Group, or Other can be represented with a single digit. Simply add up the value of each permission. Thus, **7** means read/write/execute, **6** means read/write and **5** means read/execute.

> **eg:**  
> **$** `ls -l <someFile>`  
> -rw-rw-r-- 1 user group 304 Apr 28 10:10 <someFile\>  
>
> **$** `chmod 745 <someFile>`  
> **$** `ls -l <someFile>`  
> -rwxr--r-x 1 user group 304 Apr 28 10:10 <someFile\>
