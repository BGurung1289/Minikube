# Minikube

A yaml file which will deploy an NGINX pod which will host a test webpage on a Kubernetes cluster.
The second yaml file creates a Service which allows us to expose the pod created above so it can be accessed.  

# Prerequisites
The following need to be installed:
- Kubectl
- minikube (if it is being used)


# Instructions
Start the cluster that you are going to apply the yamls to. 
For my example, I am using minikube.
``` 
minikube start -p <name> --vm-driver=virtualbox                    (this is starting the cluster)
cd into the yaml folder
kubectl create -f nginxD.yaml 
kubectl create -f svc.yaml
minikube -p <name> service nginx-svc --url
copy and paste the returned result into your web browser
```
