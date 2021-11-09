### Creare cluster
```bash
kind create cluster --config kind-config.yaml

kind delete cluster # sterge un cluster kind
```

### Rulare pod
```
kubectl run alpine --image=alpine

kubectl run -i --tty --rm alpine --image=alpine # ruleaza un pod in mod interactiv

kubectl delete pods/alpine # sterge un pod
```