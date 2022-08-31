
# Kubernetes Example




## Useful Commands

start minikube
```bash
  minikube start --driver docker
```

check status
```bash
  minikube status
```

all nodes in the cluster
```bash
  kubectl get node
```

all pods in node
```bash
  kubectl get pod
```

create config file
```bash
  kubectl apply -f mongo-config.yml
```

create secret
```bash
  kubectl apply -f mongo-secret.yml
```

start db first
```bash
  kubectl apply -f mongo.yml
```

start Web app
```bash
  kubectl apply -f webapp.yml
```

get configmap
```bash
  kubectl get configmap
```

get secret
```bash
  kubectl get all
```

list of services
```bash
  kubectl get service
```

more details of the service
```bash
  kubectl describe service <name_of_service>
```

more details of the pod
```bash
  kubectl describe pod <name_of_pod>
```

get logs
```bash
  kubectl logs <name_of_pod>
```

minikube ip
```bash
  minikube ip
```

stop minikube
```bash
  minikube stop
```

**Known issue - Minikube IP not accessible** 

If you can't access the NodePort service webapp with `MinikubeIP:NodePort`, execute the following command:
    
```bash
  minikube service webapp-service
```
