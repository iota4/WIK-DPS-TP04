Voici les fichiers de configuration d'un deployement de 4 réplicas (redondance) avec un service nginx

Pour activer mon fichier yaml de deployement & service nginx : 

```
kubectl apply -f confdeployement.yml -f my-namespace
kubectl apply -f service.yml
kubectl apply -f ingress.yml
```
Pour activer un port forwarding entre le port de la machine local et du deployement :
```
kubectl port-forward deployment.apps/mon-deployment -n my-namespace 8081:8080
```

