# Minikube

A yaml file which will deploy an NGINX pod which will host a test webpage on a Kubernetes cluster.
The second yaml file creates a Service which allows us to expose the pod created above so it can be accessed.  

# Prerequisites


# Instructions
``` 
kubectl create -f nginxD.yaml 
kubectl create -f svc.yaml
```
