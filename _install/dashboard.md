# 1. Creating sample user
```
kubectl apply -f dashboard.yml
```
# 2. Getting a long-lived Bearer Token for ServiceAccount
```
kubectl get secret admin-user -n kubernetes-dashboard -o jsonpath="{.data.token}" | base64 -d
```

# Documentation
[creating sample user](https://github.com/kubernetes/dashboard/blob/master/docs/user/access-control/creating-sample-user.md)
