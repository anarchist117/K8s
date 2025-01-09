# 1. Create SSH Tunnel
```
ssh -L8001:localhost:8001 user@remote-host
```
# 2. Start Proxy
```
kubectl proxy --port=8001
```
# 3. Getting a Bearer Token
```
kubectl -n kubernetes-dashboard create token admin-user
```
# 4. Dashboard Login
```
http://localhost:8001/api/v1/namespaces/kube-system/services/https:kubernetes-dashboard:/proxy/#/login
```


# Documentation
[Accessing Kubernetes Dashboard](https://github.com/kubernetes-sigs/kubespray/blob/master/docs/getting_started/getting-started.md#accessing-kubernetes-dashboard)
[Getting a Bearer Token for ServiceAccount](https://github.com/kubernetes/dashboard/blob/master/docs/user/access-control/creating-sample-user.md#getting-a-bearer-token-for-serviceaccount)
