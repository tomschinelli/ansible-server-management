
## Run Playbook
Note: Ensure all required hosts exists in `/etc/ansible/hosts`

All updates:
```shell
ansible-playbook site.yml --extra-vars ev_security_only=no
```
(WIP) Security updates only:
```shell
ansible-playbook site.yml --extra-vars ev_security_only=yes
```