```
git clone https://github.com/kubernetes-sigs/kubespray.git
```
```
pip3 install -r requirements.txt
```
```
cp -rfp inventory/sample/ inventory/cluster

nano inventory/cluster/inventory.ini
```
```
inventory/cluster/group_vars/all/etcd.yml
inventory/cluster/group_vars/k8s-cluster/k8s-cluster.yml
inventory/cluster/group_vars/k8s-cluster/addons.yml
inventory/cluster/group_vars/kube-ingress.yml
```
```
ansible-playbook -i inventory/cluster/inventory.ini -b --diff cluster.yml 
ansible-playbook -i inventory/cluster/inventory.ini -b --diff scale.yml
```
