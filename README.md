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

### access the termianl of any pod
kubectl exec -it <pod name> -- bin/bash

### delete deployment and all it's resources 
kubectl delete deployment <deployment name>

### get apply a deployment file
kubectl apply -f <file name>