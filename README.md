
## Run Playbook
Note: Ensure all required hosts exists in `/etc/ansible/hosts`

All updates:
```shell
ansible-playbook main.yml --extra-vars ev_security_only=no
```
Security updates only:
```shell
ansible-playbook main.yml --extra-vars ev_security_only=yes
```