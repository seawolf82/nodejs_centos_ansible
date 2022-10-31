# Nodejs_centos_ansible

Tested on:

- Almalinux 8
- Almalinux 9
- RockyLinux 8
- RockyLinux 9
- Centos 7

Tested on:

- 2.9 Ansible version


This script install on centos7 Nodejs 10 and Nodejs 16 on EL8-EL9


To install Nodejs run:

ansible-playbook -i hosts site.yaml

To uninstall Nodejs run:

ansible-playbook -i hosts deprovision.yaml

Adding Tags to permit run only specific task of playbook

Tags:

upgrade
package
nodejs
ntp

For example, to launch only task regarding upgrade os, run:
 
ansible-playbook -vv --tags "upgrade" -i hosts site.yaml
