```bash
mkdir -p $HOME/.kube
sudo cp -i /etc/kubernetes/admin.conf $HOME/.kube/config
sudo chown $(id -u):$(id -g) $HOME/.kube/config
```

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

```bash
kubectl get nodes -o wide
kubectl get namespace
kubectl get service --all-namespaces
kubectl get pods -n kube-system
```

```bash
kubectl get nodes
kubectl drain <node-name> --ignore-daemonsets
kubectl delete node <node-name>
```
