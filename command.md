```
kubectl get pod -w
kubectl get pod -o wide
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
```
