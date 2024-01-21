# Mail/Matrix Server
Contains automation and tooling to manage my own mail/matrix server.
Automated SSL generation/renewal with Let'sencrypt via cerbot and Cloudflare DNS.

## Secrets

All secrets are stored in a private Hashicorp Vault instance and fetched with ansible lookups at runtime, including the ansible host itself, this helps to keep the code clean, also allows me to keep this repo public without security concerns.
Vault Authetication must be set via ENV variables before rurring the playbook.


## Ansible

Single Step
```
ansible-playbook -i inventory.yml configure.yml --tags matrix
```

Configure Everything
```
ansible-playbook -i inventory.yml configure.yml
```


## Credits

https://www.ansible.com/ <br>
https://www.vaultproject.io/ <br>
https://github.com/element-hq/synapse <br>
https://github.com/docker-mailserver/docker-mailserver <br>
