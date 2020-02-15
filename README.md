# README

Boostrap:

```
sudo apt update
sudo apt install -y git python-pip
sudo -H pip install pip --upgrade
sudo -H pip install ansible dnspython
git clone https://github.com/paulbovbel/ansible-home.git
cd ansible-home
```

To deploy on the current machine:

`ansible-playbook -Kvvi inventory/personal playbooks/developer.yaml`

To deploy homelab:

`ansible-playbook -vvi inventory/franklin playbooks/lab.yaml`
`ansible-playbook -vvi inventory/richmond playbooks/lab.yaml`
`ansible-playbook -vvi inventory/hartleigh playbooks/lab.yaml`

TODO:
  - make a fancy login template for caddy (https://github.com/tarent/loginsrv/blob/master/README.md#templating)
