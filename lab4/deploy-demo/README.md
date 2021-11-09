# Comenzi
```bash
kubectl apply -f testapp-deploy.yaml # creeaza un deployment dintr-un fisier

kubectl get deployments # afiseaza lista cu deployment-uri

kubectl expose deployment testapp # expune un deployment ca un serviciu

kubectl get services testapp # afiseaza lista cu servicii

kubectl port-forward service/testapp 8888:5000 # mapeaza porturi in cadrul unui serviciu

```