# Installing-LAMP-on-CentOS
This is an Ansible playbook that installs LAMP (Linux, Apache, MariaDB, PHP) on CentOS.
The repo installs
- nginx
- apache
- MariaDB
- php

Requirements
- A control node
- Managed host
- Installed git
```
yum install git
```
- installed ansible
```
yum install epel-release
yum install ansible
```

Before running the play book, edit on the file "/LAMP/inventories/hosts.yaml"
```
host-ip=<your ip here>
host-user=<your user name>
```
then you can run the command
```
ansible-playbook main-playbook.yaml -i inventories/hosts
```
