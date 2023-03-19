---
id: h1h936x5ffkbeelag5zuvxm
title: Group
desc: ''
updated: 1669121088503
created: 1659193838011
---

### Creating group

Creating a new group is done with `groupadd` command.
> `groupadd <groupName>`

### Adding user to a group

This is done with `usermod`  
> `usermod -aG <groupName> <userName>`

### Removing user from a group

Removing a user from a group is somewhat difficult,  
a complete list of groups that the user is intended to be a part of must be provided and leave out the group that needed to be removed.
> `usermod -G <userName> <userGroup> <otherOptionalGroups>`

> **Note:**  
> Checking which groups a user belongs to is done with  
> `groups <userName>`

### Removing a group

A group can be removed with  
> `groupdel <groupName>`
