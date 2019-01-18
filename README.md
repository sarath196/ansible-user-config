Role Name
=========
Ansible User Config

Requirements
------------
Redhat
Centos

Installation
--------------------------
Use runsetup.yml file as host filerun playbook
```sh
$ ansible-playbook /path/runsetup.yml -i /path/inventory.txt
```
Role Variables
--------------

| Variables | Descriptions |
| ------ | ------ |
| user_name | Username (default: ansible-admin) |
| pass_code | passcode (default: admin123) |
| user_shell | usershell (default: /bin/bash) |
| ssh_conf_file | .ssh key file (default: '') |
|ssh_key_auth | allow ssh key auth (default: False) |
| user_groups | user groups (default: wheel) |
| user_timezone | user timezone (default: timedatectl set-timezone Asia/Kolkata) |
| user_enable_passwordless_sudo | user enable passwordless sudo (default: True) |

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.


Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
