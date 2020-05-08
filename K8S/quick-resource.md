# Quick Resource Provisioner

## Create Pod

```sh
kubectl run --generator=run-pod/v1 nginx --image=nginx
```

## Create Deployment

```sh
kubectl create deployment --image=nginx nginx
```
