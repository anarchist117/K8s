# Install the HAProxy Ingress Controller
```
curl https://raw.githubusercontent.com/haproxytech/kubernetes-ingress/master/deploy/haproxy-ingress-daemonset.yaml > ingress.yml
```
```
nano ingress.yml

kind: Service
spec:
  externalIPs:
  - 1.2.3.4
```
```
kubectl apply -f ingress.yml
```

# Documentation
[Install on premises](https://www.haproxy.com/documentation/kubernetes-ingress/community/installation/on-prem/)
