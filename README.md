###Usage
```shell script
sudo apt update && sudo apt -y upgrade
sudo apt install -y bash-completion python3-pip net-tools zip
pip install ansible
sudo mkdir /etc/ansible
sudo nano /etc/ansible/ansible.cfg
```
###Add following content:
[defaults]
inventory = hosts

```shell script
sudo nano /etc/ansible/hosts
```
###Add following content:

**[all]**

127.0.0.1

###Move to directory which holds playbook and run command
```shell script
ansible-playbook --connection=local --ask-become-pass playbook.yml
```
