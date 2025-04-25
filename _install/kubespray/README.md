```
apt update && apt install -y git python3-pip
```
```
git clone https://github.com/kubernetes-sigs/kubespray.git
```
```
cd kubespray/
pip3 install -r requirements.txt --break-system-packages
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
ansible-playbook -i inventory/cluster/inventory.ini cluster.yml --tags ingress
ansible-playbook -i inventory/cluster/inventory.ini scale.yml --limit NodeName
ansible-playbook -i inventory/cluster/inventory.ini remove-node.yml
ansible-playbook -i inventory/cluster/inventory.ini upgrade-cluster.yml
```
