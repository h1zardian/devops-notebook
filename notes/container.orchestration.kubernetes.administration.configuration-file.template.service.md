---
id: 6ji9ojbvb58yqqr6ynfwuv5
title: Service
desc: ''
updated: 1676874239238
created: 1676380461562
---

```yaml
apiVersion: v1
kind: Service
metadata:
  name: nginx-service
spec:
  selector:
    app: nginx #---------------a selector referencing the label values of other components that needs to be connected together
  ports:
  - protocol: TCP
    port: 80 #-----------------the listening port of the service
    targetPort: 8080 #---------matches the containerPort of the deployment 
```

### The full config file generated for the service by the Kubernetes

```yaml
apiVersion: v1
kind: Service
metadata:
  annotations:
    kubectl.kubernetes.io/last-applied-configuration: |
      {"apiVersion":"v1","kind":"Service","metadata":{"annotations":{},"name":"nginx-service","namespace":"default"},"spec":{"ports":[{"port":80,"protocol":"TCP","targetPort":8080}],"selector":{"app":"nginx"}}}
  creationTimestamp: "2023-02-20T06:14:12Z"
  name: nginx-service
  namespace: default
  resourceVersion: "18804"
  uid: 0b8c58e8-c6a4-407d-b545-dfb0101e6c7a
spec:
  clusterIP: 10.107.214.53
  clusterIPs:
  - 10.107.214.53
  internalTrafficPolicy: Cluster
  ipFamilies:
  - IPv4
  ipFamilyPolicy: SingleStack
  ports:
  - port: 80
    protocol: TCP
    targetPort: 8080
  selector:
    app: nginx
  sessionAffinity: None
  type: ClusterIP
status:
  loadBalancer: {}
```
