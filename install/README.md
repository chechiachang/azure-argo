ArgoCD
===

# Install

https://github.com/argoproj/argo-helm/tree/master/charts/argo-cd

```
kubectl create namespace argocd

helm repo add argo https://argoproj.github.io/argo-helm
helm install --namespace argocd --values values.yaml argocd argo/argo-cd
```

# Access

```
kubectl port-forward service/argocd-server -n argocd 8080:443
open http://localhost:8080
```
