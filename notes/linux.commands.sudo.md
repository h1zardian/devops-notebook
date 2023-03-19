---
id: vn82r3n8aifkfnohb2scsk7
title: Sudo
desc: ''
updated: 1659618483586
created: 1649159675840
---

## Setup

To setup sudo the user must switch to root account using `su` command.

The sudo config. file `/etc/sudoers` should always be edited with the `visudo` command.

- the default text editor for *visudo* is `vi`.  

To switch the default editor use  
>EDITOR=nano visudo

Adding a config file to `/etc/sudoers.d` folder is recommended rather than editing `/etc/sudoers`.  

Creating `/etc/sudoers.d/<your_userName>`  
>`EDITOR=nano visudo -f /etc/sudoers.d/<your_userName>`

To allow a user to gain full root privileges when they precede a command with sudo, add the following line to the file:  
> USER_NAME   ALL=(ALL:ALL) ALL

To allow a user to run all commands as any user but only on the machine with hostname HOST_NAME:  
> USER_NAME   HOST_NAME=(ALL:ALL) ALL

Setting required permissions in the shell  
> `chmod -c 440 /etc/sudoers.d/<your_userName>`

- More details:  
<https://wiki.archlinux.org/title/sudo>
