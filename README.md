Install minikube locally to run k8s cluster 

Followign are some usefull commands:

# Important commands
### start minikub
minikube start 

### get list of nodes
kubectl get nodes

### get list of nodes
kubectl get pod

### get list of replicaset
kubectl get replicaset

### get list of deployments
kubectl get deplyoment

### Create deployment
kubectly create deployment <DEPL_NAME> --image=>IMAGE_NAME>

### get log of pod
kubectl logs <pod name>

### get more information of pod like ip addresses etc.
kubectl get pod -o wide

### access the termianl of any pod
kubectl exec -it <pod name> -- bin/bash

### delete deployment and all it's resources 
kubectl delete deployment <deployment name>

### get apply a deployment file
kubectl apply -f <file name>

### get service decriptoin 
kubectl describe service <servive name>

### get auto generated staus yaml file of deployement 
kubectl get deployment <deployment name> -o yaml

### delete the deployment or service using config file 
kubectl delete -f <file path>

### assign external ip in minikute to a service 
minikue service <service name>