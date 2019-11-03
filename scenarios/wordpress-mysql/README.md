# Worodpress and MySQL

This setup requires an NFS storage that backs `PersistentVolume`. On GKE, this
can be done with Firestore.

https://stackoverflow.com/questions/54796639/how-do-i-create-a-persistent-volume-claim-with-readwritemany-in-gke

## Deployment

Edit `*-pv.yml` and set IP/Hostname of NFS server correctly.

```
kubectl apply -f .
```

> No Ingress deployed.
