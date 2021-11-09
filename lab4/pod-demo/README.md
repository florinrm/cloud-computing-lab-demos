# Comenzi

```bash
kubectl apply -f testapp-pod.yaml # creeaza un pod dintr-un fisier declarativ

kubectl port-forward testapp 8888:5000 # realizeaza mapare de porturi

kubectl logs testapp # afiseaza loguri

kubectl exec testapp -- ls # executa o comanda intr-un pod

kubectl cp file.txt testapp:/file.txt # copiaza un fisier intr-un pod

kubectl delete pods/testapp # sterge un pod
```