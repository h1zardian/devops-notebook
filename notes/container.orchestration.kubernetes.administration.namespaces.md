---
id: g653l9p499a37v8sxi297g0
title: Namespaces
desc: ''
updated: 1678042859301
created: 1676991407057
---
### Change Namespace for the current context

> `kubectl config set-context --current --namespace=dev`

### Assign Namespace while creating an object

> `kubectl [apply/run command] -n <namespace_name>`

### Assign Namespace to an object through its config file

- A namespace can be created by listing the namespace attribute in the metadata section of the config file of the object.

```yaml
apiVersion:
kind:
metadata:
  name: object_name
  namespace: namespace_name
...
...
```
