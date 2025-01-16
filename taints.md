```
kubectl describe nodes NodeName

Taints:             node-role.kubernetes.io/control-plane:NoSchedule
```
```
nano daemonset.yml

spec:
  tolerations:
  - key: "node-role.kubernetes.io/control-plane"
    operator: "Exists"
    effect: "NoSchedule"
  nodeSelector:
    node-role.kubernetes.io/control-plane: ""
```

```
kubectl taint nodes NodeName key1=value1:NoSchedule
kubectl taint nodes NodeName key1=value1:NoSchedule-
```


# Documentation
[Taints and Tolerations](https://kubernetes.io/docs/concepts/scheduling-eviction/taint-and-toleration/)
