---
id: t7s33oa4xe3q9xzw92xex5p
title: Deployments
desc: ''
updated: 1678042979244
created: 1675157357085
---

- Deployments are a kubernetes object that acts as a layer of abstraction on top of pods to make administration easier

### Creating a deployment

> `kubectl create deployment <deployment_name> --image=<image_name>:<version>`

### Editing a deployment file

> `kubectl edit deployment/deploy <deployment_name>`

- Changing the image name or version:  
>
  > ```yaml
  >spec:
  >  ....
  >  template:
  >    spec:
  >      containers:
  >      - image: <image_name>:<version>
  > ```
