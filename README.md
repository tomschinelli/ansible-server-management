
## Run Playbook

Run complete setup:
```shell
ansible-playbook site.yml -i .production
```

Create users only:
```shell
ansible-playbook site.yml --tags user -i .production
```


## Configuration
### Users :older_man:	
By default, a user `admin` is created with your default ssh public key. 
You can set up users inside `./host_vars/{hostname}.yml` or `./group_vars/{group_name}.yml`:

```yaml
# example: ./group_vars/all.yml
users:
  - name: tom
    publicKeyPath: ~/.ssh/id_rsa.pub
```