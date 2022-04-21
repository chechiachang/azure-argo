ArgoCD
===

# Install

https://github.com/argoproj/argo-helm/tree/master/charts/argo-cd

```
helmfile --selector=name=argocd diff
helmfile --selector=name=argocd apply
```

# Access

```
kubectl port-forward service/argocd-server -n argocd 8080:443
open http://localhost:8080
```
