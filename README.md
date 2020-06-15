Ansible Hardening
=================

The ansible-hardening role applies security hardening configurations from the Security Technical Implementation Guide (STIG) to systems running the following distributions:

   - CentOS 7
   - Debian Jessie
   - Fedora 27
   - openSUSE Leap 42.2 and 42.3
   - Red Hat Enterprise Linux 7
   - SUSE Linux Enterprise 12 (experimental)
   - Ubuntu 16.04

Requirements
------------

This role can be used with or without OpenStack-Ansible. It requires Ansible 2.3 or later.

Role Variable
-------------

All of the variables for this role are in defaults/main.yml.

How to Run
----------

```shell
ansible-galaxy install git+https://github.com/openstack/ansible-hardening
```

```shell
vim playbook.yml
```

        - hosts: localhost
          become: yes
          roles:
               -ansible-hardening

License
-------

Apache 2.0


Author Information
------------------

For more information, join `#openstack-ansible` on Freenode.
