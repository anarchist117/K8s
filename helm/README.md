```
helm search hub kube-ops-view --output yaml

helm repo add <repository_name>  <repository_url>
helm repo update

helm show values <repository_name>/<package_name> > values.yml

helm install <release_name> <repository_name>/<package_name> -f values.yml

helm delete <release_name>
```