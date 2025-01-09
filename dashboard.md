# 1. Create SSH Tunnel
```
ssh -L8001:localhost:8001 user@remote-host
```
# 2. Satrt proxy
```
kubectl proxy --port=8001
```
