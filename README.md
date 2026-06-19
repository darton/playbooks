# Privileged User Management (Ansible)

## Add a new privileged user
```bash
ansible-playbook -i inventory useradd.yml -e "user=wally"

or
ansible-playbook -i inventory useradd.yml -e "user=wally" -e allowed_ip="127.0.0.1"
```
## Delete a new privileged user
```bash
ansible-playbook -i inventory userdel.yml -e "user=wally"
```
