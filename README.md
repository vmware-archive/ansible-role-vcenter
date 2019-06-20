# ansible-role-vcenter

[Ansible](https://github.com/ansible/ansible) role for installing,
configuring and manipulating VMware vCenter Server objects.

## Requirements

This role currently supports Debian/Ubuntu distros.

Further, this role utilizes code that, at the creation of this role,
was currently under development at, and shared with us for our use, by,
the Ansible development team. The code base can be found at:
[github](https://raw.githubusercontent.com/ansible/ansible/devel/lib/ansible/module_utils/vmware.py)

## Role Variables

Documentation here is under way . . . in flux for a bit.

## Example playbook

```yaml
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

# License and Copyright

Copyright 2015 VMware, Inc.  All rights reserved.

SPDX-License-Identifier: Apache-2.0 OR GPL-3.0-only

This code is Dual Licensed Apache-2.0 or GPLv3

## Author Information

This role was created in 2015 by [Tom Hite, Devin Nance and Daniel Kim / VMware](http://www.vmware.com/).
