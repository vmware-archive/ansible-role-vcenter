# ansible-role-vcenter

[Ansible](https://github.com/ansible/ansible) module for installing,
configuraing and manipulating VMware vCenter Server objects.

## Requirements

This role currently supports Debian/Ubuntu distros.

Further, this role utilizes code currently under development at, and
shared by, the Ansible development team. The code base can be found at:
[github](https://raw.githubusercontent.com/ansible/ansible/devel/lib/ansible/module_utils/vmware.py)

## Role Variables

Documentation here is under way . . . in flux as the vars get integrated into SuperVIO UI.

## Example playbook

```
---
- name: create a VMware distributed switch
  hosts: local
  roles:
    - vcenter
  vars_files:
    - /vars/uianswers.yml

- name: setup portgroup in a VDS
  hosts: local
  roles:
    - vcenter
  vars_files:
    - /vars/uianswers.yml
```

## License

TBD

## Author Information

This role was created in 2015 by [Tom Hite, Devin Nance and Daniel Kim / VMware](http://www.vmware.com/).
