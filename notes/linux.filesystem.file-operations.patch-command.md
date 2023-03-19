---
id: 2xwfr270sst06o5imanfc0y
title: patch Command
desc: ''
updated: 1658331957538
created: 1658076029937
---

A patch file can be merged with any of these 2 methods.
> `patch <originalFile> <patchFile>`

> `patch -p[num] < patchFile`

**How `-p[num]` works:**

Each value of the `num` from `1-n`, strips one parent directory from the path of both files (so that if your file has a custom directory structure, it can also be patched).

```markdown
Suppose a file name is
    `/home/zardi/.config/fish/config.fish`

using `-p1` option gives
    `home/zardi/.config/fish/config.fish`

using `-p4` gives
    `fish/config.fish`

and not specifying -p at all just gives you
    `config.fish`

Whatever you end up with, is looked for either in 
the current directory or the directory specified by 
the user using option `-d`.
```
