```
git clone https://github.com/kubernetes-sigs/kubespray.git
```
```
cp -rfp inventory/sample/ inventory/cluster
```
```
pip3 install -r requirements.txt --break-system-packages
```
```
ansible-playbook -i inventory/cluster/inventory.ini cluster.yml -b -v
```
