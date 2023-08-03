

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


```
#### Generally we don't use docker in production

If somehow if container is stop working . auto healing feature is missing and auto scaling
can not use pod/containers in production

pod
api-server
pod works on node level
for one app - one deployment file


