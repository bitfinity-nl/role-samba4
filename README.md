Role Name
=========

This role contains the tasks to add an Ubuntu machine to Active Directory.

Requirements
------------

This role supports:
- Ubuntu 20.04
- Ubuntu 18.04

Role Variables
--------------

See defaults/main.yml for more information.

Dependencies
------------

See defaults/main.yml for more information.

Example Playbook
----------------

For adding additional domain controller use the example below

    - hosts: domaincontrollers
      become: yes

      vars:
        # -- Custom settings: role-samba4 --
        smb_role : 'additional'
        
      roles:
        - role-samba4

License
-------

GPLv3

Author Information
------------------

I: https://www.bitfinity.nl
E: info@bitfinity.nl

