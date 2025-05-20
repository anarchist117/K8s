```
nano ~/.bashrc

source <(kubectl completion bash)
export EDITOR=nano
alias ll='ls -la'
alias k=kubectl
complete -F __start_kubectl k
```

[Getting started](https://github.com/kubernetes-sigs/kubespray/blob/master/docs/getting_started/getting-started.md)
