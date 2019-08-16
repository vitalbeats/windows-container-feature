Windows Container Feature
=========================

This role can be used to install / remove the Windows Container feature, along with supporting docker tooling.

Requirements
------------

This role is targetted at Windows hosts only, targeting Windows Server 2016 / 2019 and Windows 10 Pro / Enterprise.

Role Variables
--------------

| Variable                           | Description                                                                             | Default Value | Required |
| ---------------------------------- | --------------------------------------------------------------------------------------- | ------------- | -------- |
| `windows_container_feature_hyperv` | Whether or not to also install the Hyper-V feature for more strict container isolation. | True          | No       |

Dependencies
------------

This role has no dependencies from Ansible Galaxy.

Example Playbook
----------------

    - hosts: windowsservers
      roles:
         - { role: stephen001.windows_container_feature, windows_container_feature_hyperv: False }

License
-------

Apache License 2.0

Author Information
------------------

Created for use by Vital Beats. http://vitalbeats.com/
