## Minikube Start
minikube start/stop/status

## Check kubectl is connected to server
kubectl cluster-info

## check kubernatic node 
kubectl get nodes

## check pods 
kubectl get pods

## create deployment
kubectl create deployment nginx(deployment name) --image=nginx:latest

## list deployments
kubectl get deployments

## list services
kubectl get services/svc

## details info of pods
kubectl describe pod pod-name

## get pod logs
kubectl logs pod-name

## go into pod
kubectl exec -it pod-name -- bash

## edit deployment
kubectl edit deployment deployment-name

## apply maniestfile
kubectl apply -f file-name.yml

## delete deployment
kubectl delete deployment deployment-name

## delete target deployment that are created from manifeast file
kubectl delete -f file-name.yaml


