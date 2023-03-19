---
id: osi33t5gpr40848jmx8f9zm
title: Commands
desc: ''
updated: 1669133864383
created: 1649135234875
---

> a command is usually in the form of  
> `<command> [option]... [arguments] OR <file>...`

- **touch** : create a file.

- **mkdir** : create a directory/ folder.

- **rm** : removes any file.

- **rmdir** : removes an entire directory.
  >the directory needs to be empty to perform rmdir.
  > Else do `rm -rf`.

- **mv** : move or rename a file/ directory.

- **cat** : used to print out contents of a file (and combine files). Alternative, `bat`.

- **man** : used to view documentation of a program.
  > **whatis** can be used to search for man pages related to a command or program.  
  > **apropos** can be used to search for all instances of command or program in the man page directory.
  >
  > `info` is also an alternative to man pages.

- **ls** : used to list the contents of a directory
  > `ls` can be used with `-a` option to list all files (hidden files also) & `-l` to get a detailed list.

- **file** : used to examine a file type with it's contents rather then extension.

- **sudo** : used to grant temporary root privilege to non-root users. See [[sudo|linux.commands.sudo]].

- **whereis** : looks throughout the filesystem to find the programs with matching name.

- **locate** : same as `whereis` but for files.

- **pwd** : prints present working directory.

- **cd** : change directory.
  >(**cd**) or (**cd ~**) : change dir to home folder.  
  >**cd ..** : change dir to the parent folder of current directory.  
  >**cd -** : change to the previous directory, you where last in.

- **history** : used to view previously executed commands.

- **tree** : displays the tree view of the file system.
  > `tree` can be used with `-d` option to just view directories in a filesystem and to suppress listing of files.

- **hostnamectl** : displays details about the system and the linux distribution.
  > Using `cat` on `/etc/os-release` will also print something similar in systems without systemd.

- **uname -srm** : displays the linux kernel version.
  > An alternative to this is `hostnamectl | grep -i kernel`.
  