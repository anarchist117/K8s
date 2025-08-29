# Change NGINX deafult settings
```
kubectl edit configmaps -n ingress-nginx ingress-nginx

apiVersion: v1
data:
  use-http2: "false"
kind: ConfigMap
```

# Restart NGINX Ingress controller
```
kubectl rollout restart daemonset -n ingress-nginx ingress-nginx-controller
```

# Verify HTTP/2 disable
```
curl -I -k --http2 https://speedtest.domain.com
```
