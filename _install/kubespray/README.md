```
git clone https://github.com/kubernetes-sigs/kubespray.git
```
```
apt install -y python3-pip
pip3 install -r requirements.txt
```
```
cp -r inventory/sample/ inventory/cluster
nano inventory/cluster/inventory.ini
```
```
group_vars/k8s-cluster/k8s-cluster.yml
group_vars/k8s-cluster/addons.yml
group_vars/kube-ingress.yml
group_vars/all/etcd.yml
```
```
ansible-playbook -i inventory/cluster/inventory.ini --diff cluster.yml 
ansible-playbook -i inventory/cluster/inventory.ini --diff scale.yml
ansible-playbook -i inventory/cluster/inventory.ini --diff remove-node.yml
ansible-playbook -i inventory/cluster/inventory.ini --diff upgrade-cluster.yml
```
