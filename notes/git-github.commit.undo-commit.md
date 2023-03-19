---
id: 9fhvarpse5eywi80k66lmac
title: Undo Commit
desc: ''
updated: 1668870070675
created: 1668005685404
---

### Undo the commit once

> `git reset HEAD~1`

### Revert commits to a certain point

> `git log`  
> \* git logs every commit with a hash, that can be used to revert back to any pervious commits

> `git reset <hash-of-the-destination-commit>`  
> \* This will revert the commit but all the code changes will still be saved in the editor

### Revert commits to a certain point and delete unsaved changes

> `git reset --hard <hash-of-the-destination-commit>`  