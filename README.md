```
nano ~/.bashrc

source <(kubectl completion bash)
export EDITOR=nano
alias ll='ls -la'
alias k=kubectl
complete -F __start_kubectl k
```

```bash
kubectl get nodes -o wide
kubectl get namespace
kubectl get service --all-namespaces
kubectl get pods -n kube-system
```

https://github.com/kubernetes-sigs/kubespray/blob/master/docs/getting_started/getting-started.md
