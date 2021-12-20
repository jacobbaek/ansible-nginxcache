# deploy logging and monitoring service using Ansible

# Support OS
* Ubuntu 20.04

# How to use

Choice the tag and write the tag with ansible-playbook command.
```
# monitoring : prometheus, grafana, exporters
ansible-playbook -i inventory/inventory.ini site.yml -t monitoring

# logging : loki, promtail, grafana
ansible-playbook -i inventory/inventory.ini site.yml -t logging
```

if want to deploy one software, add the 'once' tag in the site.yml
```
ansible-playbook -i inventory/inventory.ini site.yml -t once
```
