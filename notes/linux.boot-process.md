---
id: n8h91c1lg16yiaqys8c5ej1
title: Boot Process
desc: ''
updated: 1653731511142
created: 1648996282262
---
---

![Boot Process](assets/images/boot-process-flowchart.jpg){float: right, max-width: 50%}

### Bios

- Basic Input/ Output System
- Resides on a rom chip on motherboard.

### Bootloader

- Bootloader is either stored in the `MBR` (Master Boot Record) sector of the hard drive or the `UEFI` (Unified Extensible Firmware Interface) partition.

- It resides under the `/boot` directory and uses the **partition table** to find a bootable partition on the disk. After which it loads the [[kernel|linux.kernel]] as well as `initramfs` into the RAM and passes the system control to it.

- Some notables bootloaders are `GRUB` (GRand Unified Bootloader), `ISOLINUX` for removable devices and `DAS U-Boot` for embedded devices.

### initramfs

Initial RAM File System

- It's job is to mount the filesystem and device drivers to correct places and signal the [[kernel|linux.kernel]] that the root filesystem is ready to use.

### /sbin/init

> `/sbin/init` now just points  
> to `/lib/systemd/systemd`

- It is the initial process for the operating system as it starts other processes to get the system running.

- `init` is in itself a daemon with the job to start and stop all other process, daemon and services (except the kernel processes) cleanly and reliably for the operating system.

- Some well-known `init` daemons are [[systemd|linux.systemd]], `OpenRC`, `runit` etc.

- useful `systemd` [[commands|linux.systemd#commands]].
