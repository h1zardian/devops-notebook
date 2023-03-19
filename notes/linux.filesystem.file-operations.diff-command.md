---
id: h42n0r6mgth7fy8i2w7msh6
title: diff Command
desc: ''
updated: 1658160461342
created: 1658071311871
---

### diff

Used to compare 2 files, at the command prompt.

> `diff [options] <fileName1> <fileName2>`

**Options :**  
    `-c` : prints the difference with three lines of context before and after the differing line.  
    `-i` : ignore the cases of letters.  
    `-w` : ignore differences in spaces and tabs.  
    `-q` : only report if the files are different without listing the difference (Quite Mode).  

> `diff` is only meant to be used for text files.  
> for binary files, use `cmp`.

</br>

**Creating Patch file with diff :**  
`diff` can be used to create a patch file that may only contain the changes that you have made. Use [[patch|linux.filesystem.file-operations.patch-command]] command to merge it with original file.

> `diff -u originalFile updatedFile > patchFile`

### diff3

- Used to compare two modified files with a reference file (comparing three files at once).

> `diff3 <file1> <referenceFile> <file2>`
