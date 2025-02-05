```
kubectl describe nodes control1

Taints:             node-role.kubernetes.io/control-plane:NoSchedule
```
```
nano deployment.yml

spec:
  tolerations:
  - key: "node-role.kubernetes.io/control-plane"
    operator: "Exists"
    effect: "NoSchedule"
  nodeSelector:
    node-role.kubernetes.io/control-plane: ""
```

```
kubectl taint nodes control1 key1=value1:NoSchedule
kubectl taint nodes control1 key1=value1:NoSchedule-
```


# Documentation
[Taints and Tolerations](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
