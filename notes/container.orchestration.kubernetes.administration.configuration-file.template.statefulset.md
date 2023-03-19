---
id: uwgw33s97hz0c9w5u8jcw29
title: StatefulSet
desc: ''
updated: 1678631414421
created: 1678630574694
---

```yaml
apiVersion: app/v1
kind: StatefulSet
metadata:
  name: web
spec:
  serviceName:  "nginx"
  replicas: 2
  selector:
    matchLabels:
      app: nginx
  template:
    metadata:
      labels:
        app: nginx
    spec:
      containers:
      - name: nginx
        image: k8s.grc.io/nginx-slim:0.8
        ports:
        - containerPort: 80
          name: web
        volumeMounts:
        - name: www
          mountPath: /usr/share/nginx/html
  volumeClaimTemplates:
  - metadata:
      name: www
    spec:
      storageClassName: local-path
      accessModes: ["ReadWriteOnce"]
      resources:
        requests:
          storage: 1Gi
```

### Headless service for the stateful set

```yaml
apiVersion: v1
kind: Service
metadata:
  name: nginx
  labels:
    app: nginx
spec:
  ports:
  - port: 80
    name: web
  clusterIP: None #-----------------a null IP is what makes a service headless
  selector:
    app: nginx
```
