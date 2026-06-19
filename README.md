# Privileged User Management (Ansible)

## Add a new privileged user
```bash
ansible-playbook -i inventory useradd.yml -e "user=wally"
```
or
```bash
ansible-playbook -i inventory useradd.yml -e "user=wally" -e allowed_ip="127.0.0.1"
```
or
```bash
ansible-playbook -i inventory useradd.yml -e user=wally -e allowed_ip="127.0.0.1" -e ssh_pub_key=~/.ssh/id_ed25519.pub
```

## Delete a privileged user
```bash
ansible-playbook -i inventory userdel.yml -e "user=wally"
```
