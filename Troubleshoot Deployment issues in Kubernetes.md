Last week, the Nautilus DevOps team deployed a redis app on Kubernetes cluster, which was working fine so far. This morning one of the team members was making some changes in this existing setup, but he made some mistakes and the app went down. We need to fix this as soon as possible. Please take a look.

The deployment name is redis-deployment. The pods are not in running state right now, so please look into the issue and fix the same.

Note: The kubectl utility on jump_host has been configured to work with the kubernetes cluster.

Solution
========
```
kubectl get pods
```
```
kubectl get deployment 
```
```
kubectl get configmap

```
```
kubectl describe deployment
```
```
kubectl describe configmap
```
```
kubectl describe pods
```

```

kubectl edit deployment # correct the name from "cofig to config"  and "alpin to alpine"by searching witht he pattern "/config" and "/alpin"
```

Verification
```
kubectl get deployment
```
```
kubectlt get pod
```
