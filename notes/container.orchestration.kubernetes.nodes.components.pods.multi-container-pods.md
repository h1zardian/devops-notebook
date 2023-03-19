---
id: pfbvcx5uom0o0j4cedlonx5
title: multi-container pods
desc: ''
updated: 1678170666365
created: 1678169165242
---

- A multi-container pod has one or more containers running inside the same pod.

- An auxiliary container can be used to log the main application logs, or there can be a helper container that can be used to act as a reverse proxy and host the static files from the main container, or it can be used to send out network traffic to the outside world.

### Get logs of one container from the multi-container pod

> `kubectl logs -f <pod_name> -c <container_name>`
