# k8spod2nfs
Shared persistent NFS storage for pods

##
```
docker build -t javiermugueta/k8spod2nfs .

docker push javiermugueta/k8spod2nfs
```

##
```
kubectl apply -f k8spod2nfs.yaml

kubectl get pods

kubectl exec -it k8spod2nfs-6f48c6464f-j9jrt bash
cd /usr/share/nginx/html/
echo hola > index.html

kubectl get services

echo adios  > index.html

kubectl delete pod -l app=k8spod2nfs

kubectl delete -f k8spod2nfs.yaml
kubectl apply -f k8spod2nfs.yaml

```
