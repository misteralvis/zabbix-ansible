# README #

## What is this repository for? ##

This repository holds Ansible roles/playbooks that can be used to deploy Zabbix Infrastructure.

Agents, Proxies, and eventually Server Roles will be supported.

Local Server databases can also be supported, but are generally out-of-scope to pure Zabbix Infrastructure, as they could be managed (ie, RDS) or externally accessible. 

## How do I use these roles/playbooks? ##

### Example: zabbix-proxy ###
```
#--- Use a host_vars files to specify unique values for a given build
ansible-playbook setup_zabbix_proxy.yml --extra-vars @host_vars/zabbix-proxy-template.yml --check --diff
ansible-playbook setup_zabbix_proxy.yml --extra-vars @host_vars/zabbix-proxy-template.yml
```
