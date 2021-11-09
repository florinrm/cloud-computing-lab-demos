# Comenzi
```bash
kubectl apply -f testapp-rs.yaml # creeaza un ReplicaSet dintr-un fisier

kubectl get replicasets # afiseaza lista de ReplicaSet-uri

kubectl describe rs testapp # afiseaza detalii despre un ReplicaSet

kubectl scale replicasets testapp --replicas=4 # scaleaza un ReplicaSet

kubectl apply -f testapp-rs.yaml # aplica modificari asupra unui ReplicaSet

kubectl delete rs testapp # sterge un ReplicaS
```