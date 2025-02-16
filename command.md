```
kubectl get pod -w
kubectl get pod -o wide
kubectl get pods --all-namespaces -l app.kubernetes.io/name=ingress-nginx --watch
```
```
kubectl describe pod <pod_name>
```
```
kubectl get configemaps
```
```
kubectl exec -it <pod_name> -- bash
kubectl exec <pod_name> -- cat /etc/nginx/conf.d/default.conf
```
```
kubectl port-forward <pod_name> 20000:80 &
kubectl port-forward service/<service-name> 20000:80
```
```
kubectl get service
kubectl get endpoints
```
```
kubectl scale deployment "deployment_name" --replicas=3
```
```
kubectl get ingress
```
```
kubectl get namespaces
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
kubectl get componentstatuses
```
```
kubectl exec --namespace kube-system nginx-ingress-controller cat /etc/nginx/nginx.conf
```
```
kubectl get node <node_name> -o yaml
```
```
kubectl get pvc
```
```
kubectl config set-context --current --namespace NamespaceName
```
