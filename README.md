# Nginx server on Kubernates
We use deployment to run an nginx container from nginx:alpine image and we use a  service (type loadBlanacer) to expose the server.

```
kubectl create -f nginx.deployment.yml
kubectl apply -f nginx.service.yml
```

get informations you like:
```
kubectl get all
kubectl get pods -o wide
kubectl describe svc my-nginx
```


ssh to a pod:
```
Kubectl exec [pod-name] -it sh
```
