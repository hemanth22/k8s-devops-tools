Command to create namespace

```
kubectl create namespace devops-tools
```

Command to deploy nexus3 in kubernetes

```
kubectl create -f sonatype.yaml
```

Command to check status of nexus3

```
kubectl get all -n devops-tools
```

Command to check pods status of nexus3  

```
kubectl get pod -n devops-tools
```

Command to expose service from minikube

```
minikube service nexus-service -n devops-tools
```

Command to execute commands in pods

```
kubectl exec -it pod/nexus-68bb9b6b87-gz7bw -n devops-tools -- /bin/bash
```

Command to delete Deployment

```
kubectl delete -f sonatype.yaml
```
