# Install the HAProxy Ingress Controller
```
curl https://raw.githubusercontent.com/haproxytech/kubernetes-ingress/master/deploy/haproxy-ingress.yaml > ingress.yml
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
[Install on premises](https://www.haproxy.com/documentation/kubernetes-ingress/community/installation/on-prem/)
