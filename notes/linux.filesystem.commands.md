---
id: a2wbr190eqrr1errzx1l4ak
title: Commands
desc: ''
updated: 1660905262923
created: 1658071642495
---

### Navigating directory history

**pushd & popd** :  

- `pushd .` adds directories to a stack which can be iterated through by using `pushd +/-<num>`.
- to remove a directory from the stack use `popd`.
- use the `dirs` commands to print the directory stack.

**cdh** for fish shell : it allows you to list recently visited directories and quickly navigating through by their numeral entries.

</br>

### Managing files

**find** : it lists all files in the current directory as well as all its subdirectories.  

- Options:  
    `-name` : use wildcards to search for a file.  
    `-type` : `d` for directory, `f` for file & `l` for symbolic link.

> *eg.*  
> find /usr -name gcc-* -type f

**tac** : prints out a file backwards, starting with the last line.

**less** : used to view large files, provides scroll-back capabilities.

**ln -s** : used to create symlink or symbolic link of a file.

**head** : used to show the first few lines of a file.
> To print the first 5 lines  
> `head -n 5 <fileName>`

**tail** : used to show the last few lines of a file.
> To print the last 15 lines  
> `tail -15 <fileName>`  

> **Note** :  
>
> `tail` can also be used to monitor a continuous growing file, like a oncoming log file.  
> `tail -f <logFile>`
