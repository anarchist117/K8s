# Install Ingress controller
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
[Ingress](https://kubernetes.io/docs/concepts/services-networking/ingress/)

[Bare-metal considerations](https://github.com/kubernetes/ingress-nginx/blob/main/docs/deploy/baremetal.md)
