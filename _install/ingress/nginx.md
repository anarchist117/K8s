# Install the Ingress-Nginx Controller
```
curl https://raw.githubusercontent.com/kubernetes/ingress-nginx/main/deploy/static/provider/baremetal/deploy.yaml > ingress.yml
```
```
nano ingress.yml

kind: Service
spec:
  type: NodePort => ClusterIP
  externalIPs:
  - 1.2.3.4

kind: Deployment => DaemonSet
```
```
kubectl apply -f ingress.yml
```

# Documentation
[Installation Guide](https://kubernetes.github.io/ingress-nginx/deploy/)

[Bare-metal considerations](https://github.com/kubernetes/ingress-nginx/blob/main/docs/deploy/baremetal.md)
