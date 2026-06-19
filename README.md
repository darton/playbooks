# Privileged User Management (Ansible)

## Add a new privileged user
```bash
ansible-playbook -i inventory useradd.yml -e "user=wally"
```
## Delete a new privileged user
```bash
ansible-playbook -i inventory userdel.yml -e "user=wally"
```
