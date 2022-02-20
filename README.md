###Usage
```shell script
sudo nano /etc/ansible/hosts
```
###Add following content:

**[all]**

127.0.0.1

###Move to directory which holds playbook and run command
```shell script
ansible-playbook playbook.yml --connection=local
```
