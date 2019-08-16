Windows Container Feature
=========================

This role can be used to install / remove the Windows Container feature, along with supporting docker tooling.

Requirements
------------

This role is targetted at Windows hosts only, targetting Windows Server 2016 / 2019. It uses Cmdlets that would not necessarily be available on Windows 10.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

This role has no dependencies from Ansible Galaxy.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

Apache License 2.0

Author Information
------------------

Created for use by Vital Beats. http://vitalbeats.com/
