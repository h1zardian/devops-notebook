---
id: 86dn67x0osodzw2i7u5wkx7
title: Commands
desc: ''
updated: 1678544165332
created: 1675690854470
---

> most commands are in the form of  
> `kubectl [option]...`

- **kubectl version -o yaml** : prints the version details of client and server in the yaml format.

- **kubectl get nodes | pods | services | replicasets | deployments** : lists all the available objects from the particular component in the cluster.

  > get more info out of the `kubectl get` command with `-o wide` flag.

- **kubectl describe `<component_name> <resource_name>`**: prints a detailed description and events of the selected object.

- **kubectl rollout `<subcommand>`**: manage the rollout of one or many kubernetes resources.

- **kubectl scale --replicas=`<desired_state> <component_name> <resource_name>`**: set a new size for a deployment, replica set, replication controller, or stateful set.
