# DevConf Demo Ansible 202

Dummy Ansible Role to show how molecule works.

## Requirements

- Internet
- Ansible
- Molecule

## Dependencies

- ezlee.ansible-helloworld

Example Playbook

- hosts: servers
  roles:
     - role: check_ansible_version

## How to try it?

- Clone this repo
- Prepare a Virtualenv with molecule and load it
- execute molecule

```
virtualenv -p python .virtualenv
source .virtualenv/bin/activate
pip install molecule
ansible-galaxy install -r molecule/default/requirements.yml
molecule test
```

## License

Beerware

## Author Information

[Juan Manuel Parrilla](https://twitter.com/Kerbeross)


