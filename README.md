# self-hosted-stuff
Contains automation and tooling to manage many self hosted things.

## Usage

Check
```
ansible-playbook -i inventory.yml configure.yml -e @vault.yml --check
```

Configure
```
ansible-playbook -i inventory.yml configure.yml -e @vault.yml
```
