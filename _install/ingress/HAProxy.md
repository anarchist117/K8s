# Install the HAProxy Ingress Controller
```
curl https://raw.githubusercontent.com/haproxytech/kubernetes-ingress/master/deploy/haproxy-ingress-daemonset.yaml > ingress.yml
```
```
nano ingress.yml

kind: Service
spec:
  type: NodePort => ClusterIP
  externalIPs:
  - 1.2.3.4

kind: Deployment => DaemonSet
spec:
  template:
    spec:
      containers:
        ports:
        - name: http
          containerPort: 8080
          hostPort: 8080 => 80
        - name: https
          containerPort: 8443
          hostPort: 8443 => 443
        - name: stat
          containerPort: 1024
          hostPort: 1024
```
```
kubectl apply -f ingress.yml
```

# Documentation
[Install on premises](https://www.haproxy.com/documentation/kubernetes-ingress/community/installation/on-prem/)
