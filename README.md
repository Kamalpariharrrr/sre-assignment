# SRE Assignment – Metrics App Deployment

1. **Setup**: Use Docker Desktop, VS Code, Git, KIND, ArgoCD, and Helm.
2. **Create KIND Cluster**: `kind create cluster --name sre-cluster`.
3. **Install ArgoCD**: `kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml`.
4. **Create Helm Chart**: Define image and secret in `metrics-app`.
5. **Deploy via ArgoCD**: Connect GitHub repo to ArgoCD UI.
6. **Expose via Ingress**: `kubectl apply -f ingress-nginx.yaml`.
7. **Testing**: `curl http://localhost/counter` returns incrementing values.
8. **Debug**: Resolve Docker issues, Pending pods, and ingress routing.
9. **Root Cause**: Docker not running or insufficient resources.
10. **Conclusion**: App deployed successfully, `/counter` works correctly.
