# deploy cache and origin servers using Ansible

# Support OS
* Ubuntu 20.04

# How to use

Choice the tag and write the tag with ansible-playbook command.
```
# cache : nginx cache servers
ansible-playbook -i inventory/inventory.ini site.yml -t cache

# origin : nginx origin servers
ansible-playbook -i inventory/inventory.ini site.yml -t origin
```

