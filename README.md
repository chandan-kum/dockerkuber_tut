## Minikube Start
minikube start/stop/status

## Check kubectl is connected to server
kubectl cluster-info

## check kubernatic node 
kubectl get nodes

## check pods 
kubectl get pods (it show pods in default namespace) / kubectl get pods -n namespace-name

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

## list pod with additional details
kubectl get pods -o wide

## list namespaces
kubectl get ns

## Get the specific pods which falls under the namespaces
kubectl get pods -n namespace-name

## create the namespace
kubectl create namespace/ns namespace_name

## delete namespaces 
kubectl delete namespace/ns namespace_name

## check kubernatic api resources
kubectl api-resources | grep specific-name

## get lable of namespace
kubectl get ns --show-labels

## describe namespace
kubectl describe namespace/ns namespace-name

## Argocd port forwording
kubectl port-forward service/my-argo-cd-argocd-server -n argocd 8081:443

