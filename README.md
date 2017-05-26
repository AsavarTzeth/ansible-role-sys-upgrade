Ansible Users Role - ansible-role-sys-upgrade
=============================================

**Ansible role that manages package upgrades and optionally reboots if
neccessary.**

Requirements
------------

This role was developed and tested on Ansible 2.2.0 and higher.
It may work on lower versions but that is currently unsupported.

Role Variables
--------------

    # Will check if the system requires a reboot and act upon it
    sys_upgrade_reboot:  (default: false)

Dependencies
------------

None

Example Playbook
----------------

When upgrades are complete, reboot if neccessary

    - hosts: all
      roles:
        - role: AsavarTzeth.sys-upgrade
          sys_upgrade_reboot: true

License
-------

BSD-2-Clause

Author Information
------------------

Patrik Nilsson
