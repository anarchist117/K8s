# Install Ingress controller
```
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/main/deploy/static/provider/baremetal/deploy.yaml
```

# Verify access
```
curl <worker-external-ip>:<node-port> -H 'Host: web.domain.com'
```

# Documentation
[Ingress](https://kubernetes.io/docs/concepts/services-networking/ingress/)

[Bare-metal considerations](https://github.com/kubernetes/ingress-nginx/blob/main/docs/deploy/baremetal.md)
