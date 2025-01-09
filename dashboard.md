# 1. Create SSH Tunnel
```
ssh -L8001:localhost:8001 user@remote-host
```
# 2. Start proxy
```
kubectl proxy --port=8001
```
# 3. Connect to Dashboard
```
http://localhost:8001/api/v1/namespaces/kube-system/services/https:kubernetes-dashboard:/proxy/#/login
```
