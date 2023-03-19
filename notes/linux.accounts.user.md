---
id: 0dosxzqib7ybydflh4p5qbk
title: User
desc: ''
updated: 1659541157991
created: 1659193818832
---

### Adding a user

Adding any user is done with the `useradd` command.  
> `useradd <userName>`

> **Note:**  
> `useradd` doesn't create user directories or configures any permission by default. The admin will have to use multiple flags and options to add additional information (passwords, permissions, etc.).

### useradd alternative

`adduser` is a perl script with `useradd` at the backend, with an extensive config options. Which automatically sets up a user directory with necessary files in the home folder.

### Removing a user

Any user can be removed with `userdel` command.

> **Note:**  
> Using the `userdel` will leave the user directory intact. To remove the user home directory while removing the account, use `-r` option with `userdel`.
