- https://github.com/kubernetes/dashboard/blob/master/docs/user/access-control/creating-sample-user.md

```
kubectl -n kubernetes-dashboard describe secret $(kubectl -n kubernetes-dashboard get secret | grep admin-user | awk '{print $1}')
```