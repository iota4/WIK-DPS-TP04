Voici les fichiers de configuration d'un deployement de 4 réplicas avec un service nginx

Pour activer mon fichier yaml de deployement/service nginx : 

```
kubectl apply -f confdeployement.yml -f my-namespace
kubectl apply -f service.yml
kubectl apply -f ingress.yml

