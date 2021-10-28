Katello Client Uplaod
=========

This role installs katello-host-tools and runs commands to force the katello tools to upload latest package and repo information to Satellite.

Requirements
------------

It is assumed that katello-agent is installed on the destination.

Role Variables
--------------

No

Dependencies
------------

Nil.

Example Playbook
----------------

```yaml
---
- name: Force Katello client tools to upload to Satellite
  hosts: all
  gather_facts: no
  tasks:
    - name: Apply Katello client upload role
      include_role:
        name: katello_client_upload
```
License
-------

BSD

Author Information
------------------

Blake Douglas, blake@redhat.com
