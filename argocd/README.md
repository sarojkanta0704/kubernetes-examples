Reference: https://github.com/argoproj/argo-cd/blob/master/manifests/install.yaml


To fix err_too_many_redirects issue: https://stackoverflow.com/questions/49856754/nginx-ingress-too-many-redirects-when-force-ssl-is-enabled

Default PWD: 
```bash
kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d
```