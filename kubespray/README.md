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
group_vars/k8s-cluster/k8s-cluster.yml
group_vars/k8s-cluster/addons.yml
group_vars/kube-ingress.yml
group_vars/all/etcd.yml
```
```
ansible-playbook -i inventory/cluster/inventory.ini -b --diff cluster.yml 
ansible-playbook -i inventory/cluster/inventory.ini -b --diff scale.yml
ansible-playbook -i inventory/cluster/inventory.ini -b --diff upgrade-cluster.yml
```
