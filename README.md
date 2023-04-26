# create an ansible inventory
```
[all:vars]
ansible_user=superuser
ansible_sudo_pass=changeme
k8s_version=1.25.8
pod_cidr=192.168.0.0/16
api_adv_addr=10.0.0.10
extra_sans=m1.home.lab
calico_version=v3.25.1
metallb_version=v0.13.9
ip_range=10.0.0.31-10.0.0.40
certmanager_version=v1.11.0
root_crt=/Users/ysung/git/homelab/root.crt
root_key=/Users/ysung/git/homelab/root.key
kubeconf=/Users/ysung/.kube/config
keycloak_version=21.1.0
[master]
m1.home.lab

[workers]
w[1:4].home.lab
nuc9.home.lab
p3.home.lab
```
# create a self-sign ca key/cert
# prepare sn-license.txt
# run ansible-playbooks
