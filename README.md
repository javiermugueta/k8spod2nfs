#

##
```
docker build -t javiermugueta/k8spod2nfs .

docker push javiermugueta/k8spod2nfs
```

##
```
kubectl apply -f k8spod2nfs.yaml

kubectl delete -f k8spod2nfs.yaml
```
