# Wordpress and MySQL

* Uses cloud backed PVC. Cannot use replicas > 1 as most cloud block storage do not allow `ReadWriteMany`
* Use `LoadBalncer` to expose Wordpress service outside cluster

## Deployment

```
kubectl apply -f .
```

> No Ingress deployed.
