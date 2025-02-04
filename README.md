```
kubectl completion bash > k8s.sh
```
```
nano k8s.sh

alias k=kubectl

if
  complete -o default -F __start_kubectl kubectl
  complete -o default -F __start_kubectl k
else
  complete -o default -o nospace -F __start_kubectl kubectl
  complete -o default -o nospace -F __start_kubectl k
```
```
cp k8s.sh /etc/profile.d/
bash
```

```
nano ~/.bashrc
export EDITOR=nano
```

```bash
kubectl get nodes -o wide
kubectl get namespace
kubectl get service --all-namespaces
kubectl get pods -n kube-system
```

https://github.com/kubernetes-sigs/kubespray/blob/master/docs/getting_started/getting-started.md
