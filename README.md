
#### Auto scaling and auto healing is missing in docker

```

minikube start --driver=docker
minikube ssh
exit
sudo snap install kubectl --classic
kubectl get pods
kubectl get pods --namespace=kube-system
kubectl get namespaces
kubectl create namespace springboot-app
kubectl apply -f pod.yaml
kubectl get nodes
kubectl delete -f pod.yaml
kubectl delete pods -n django-todo-app django-todo-pod
kubectl delete pods django-app-deployment-56674cb698-9hchq
kubectl delete -f .\deploy.yaml
kubectl apply -f .\deploy.yaml
kubectl get pods -n django-todo-app -o wide
kubectl get pods --namespace=django-todo-app
kubectl apply -f .\service.yaml
minikube service djangoservice -n django-todo-app --url 
minikube config set driver hyperv

```
#### Generally we don't use docker in production

If somehow if container is stop working . auto healing feature is missing and auto scaling
can not use pod/containers in production

pod
api-server
pod works on node level
for one app - one deployment file



### Run Redis


```
minikube service redis-service --url
redis-cli -h 127.0.0.1 -p 60751
```



