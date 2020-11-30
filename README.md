# Ansible Role - Python PIP

![abandoned](https://img.shields.io/badge/project-abandoned-red)

Python PIP with Development Tools and automatic PIP Upgrade

## Requirements

This role requires Ansible 2.0 or higher, and platform requirements are listed in the metadata file.

## Example Playbook

```
- hosts: localhost
  roles:
    - role: elnebuloso.pip
```

## Dependencies

None.

##  License

MIT

## Other

### Update all PIP Packages

```
pip freeze --local | grep -v '^\-e' | cut -d = -f 1  | xargs -n1 pip install -U
```

##  Author Information

This role was created in 2017 by [elnebuloso](https://github.com/elnebuloso/)