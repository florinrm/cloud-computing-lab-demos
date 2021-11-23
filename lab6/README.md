# Laborator 6 - comenzi

```bash

# first part

kind create cluster --config kind-config-three-nodes.yaml # cream cluster-ul

kubectl apply -f nginx.yaml # pornim un pod

kubectl run nginx --image=nginx --dry-run=client -o yaml # nu se porneste nimic, avem un output YAML

kubectl delete pod nginx

# second part
kubectl run nginx --image=nginx --port=8080 --dry-run=client -o yaml > test.yaml # apoi punem label-ul app:myapp

kubectl apply -f test.yaml

kubectl apply -f nginx-service.yaml

kubectl get all

kubectl describe pod nginx

kubectl describe service nginx

kubectl delete pod nginx

kubectl delete service nginx

kubectl apply -f nginx-deployment.yaml

kubectl delete deployment.apps/nginx-deployment

# last part

kubectl run db --image=mobylab/cc-laborator5-db --dry-run=client -o yaml > db-pod.yaml

kubectl apply -f db-pod.yaml

kubectl apply -f db-service.yaml

kubectl get all

kubectl run rabbitmq --image=rabbitmq:3 --port=5672 --dry-run=client -o yaml > queue-pod.yaml

kubectl apply -f queue-pod.yaml

kubectl apply -f queue-service.yaml

kubectl run procesator --image=mobylab/cc-laborator5-proc --dry-run=client -o yaml > procesator-pod.yaml

kubectl apply -f procesator-pod.yaml

kubectl run api --image=mobylab/cc-laborator5-api --dry-run=client -o yaml > api-pod.yaml

kubectl apply -f api-pod.yaml

kubectl apply -f nodeport-pod.yaml

kubectl port-forward service/api-nodeport-service 8000:8000
```
