```
kubectl get pods -w -o wide
kubectl get pods --all-namespaces -l app.kubernetes.io/name=ingress-nginx --watch

kubectl get ingress
kubectl get service --all-namespaces
kubectl get endpoints

kubectl get namespaces
kubectl get componentstatuses
kubectl get node <node_name> -o wide
kubectl get configemaps
kubectl get pvc
```
```
kubectl describe pod <pod_name>
```
```
kubectl exec -it <pod_name> -- bash
kubectl exec <pod_name> -- cat /etc/nginx/conf.d/default.conf

kubectl exec --namespace kube-system nginx-ingress-controller cat /etc/nginx/nginx.conf
```
```
kubectl port-forward <pod_name> 20000:80 &
kubectl port-forward service/<service-name> 20000:80
```
```
kubectl scale deployment "deployment_name" --replicas=3
```
```
kubectl delete -f .
kubectl delete pods -n longhorn-system --field-selector=status.phase=Failed
```
```
kubectl explain pod
kubectl api-resources
```
```
kubectl config set-context --current --namespace NamespaceName
```
```
kubectl patch namespace longhorn-system -p '{"spec":{"finalizers":null}}' --type=merge
```
