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
group_vars/all/etcd.yml
group_vars/k8s-cluster/k8s-cluster.yml
```
```
ansible-playbook -i inventory/cluster/inventory.ini cluster.yml -b -v
```
