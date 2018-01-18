# DevConf.cz 2018 - Ansible 202

Dummy Ansible Role to show how molecule works.

## Requirements

- Internet
- Ansible
- Molecule

## Dependencies

- ezlee.ansible-helloworld

Example Playbook

```
- hosts: servers
  roles:
     - role: check_ansible_version
```

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

## References

- [Juan Manuel Parrilla](https://twitter.com/Kerbeross)
- [Talk Description](Ansible202-DevConf.md)
- [Testing roles with TravisCI](https://www.jeffgeerling.com/blog/testing-ansible-roles-travis-ci-github)
- [Testing Roles on multiple OS](https://www.jeffgeerling.com/blog/2016/how-i-test-ansible-configuration-on-7-different-oses-docker)
- [Testing Roles with Docker](https://www.ansible.com/blog/testing-ansible-roles-with-docker) 
- [Molecule Docs](https://molecule.readthedocs.io/en/latest/usage.html)
- [Molecule Repo](https://github.com/metacloud/molecule)
