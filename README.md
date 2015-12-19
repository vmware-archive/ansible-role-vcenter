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

Copyright 2015 VMware, Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

## Author Information

This role was created in 2015 by [Tom Hite, Devin Nance and Daniel Kim / VMware](http://www.vmware.com/).
