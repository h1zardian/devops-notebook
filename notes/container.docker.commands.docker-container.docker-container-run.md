---
id: 4go3onosc0h29aw8amz2dm9
title: docker container run
desc: ''
updated: 1672318082319
created: 1670423954794
---

> **legacy command** :  
> `docker run`

### Create and start a new container with an image

> `docker container run <image_name>:<version>`
>
> \* this command by default checks locally for the specified image, but it can pull one if the specified image or the version is not available locally

### Create new container and launch interactive terminal

> `docker -it <image_name>:<version>`

### Create new container in detached mode

> `docker container run -d <image_name>:<version>`

### Create a new container with a custom name

> `docker container run --name <custom_name> <image_name>:<version>`

### Create a new container with custom port binding

> `docker container run -p <host_port>:<container_port> <image_name>:<version>`
