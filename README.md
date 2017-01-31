ansible-ntp
===========

[![Build Status](https://travis-ci.org/galexrt/ansible-ntp.svg?branch=master)](https://travis-ci.org/galexrt/ansible-ntp)

Ansible role to setup the NTP client.

Requirements
------------

No special requirements.

Role Variables
--------------

See the file `default/main.yml`, for available variables.

Dependencies
------------

No dependencies.

Example Playbook
----------------

To use this role you add the following as the name of the role:
```
- hosts: servers
  roles:
    - { role: galexrt.ntp }
```

License
-------

Apache 2.0 License

Author Information
------------------

If you have problems with the role, feel free to create an issue on Github or contact me by mail.
