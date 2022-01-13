# flask-k8s

To view app in browser:
```
eval $(minikube -p minikube docker-env)
docker build -t flask-k8s .
kubectl apply -f k8s/
kubectl port-forward svc/flask-k8s 9000:80
```

In browser:
```
localhost:9000
```