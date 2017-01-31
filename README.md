ansible-ntp
===========

[![Build Status](https://travis-ci.org/galexrt/ansible-ntp.svg?branch=master)](https://travis-ci.org/galexrt/ansible-ntp)

Ansible role to setup the NTP client.

Requirements
------------

No special requirements.

Role Variables
--------------

```
# This hast to be a list of existing inventory groups or false to just use the ntp_servers
ntp_server_groups:
  - ntp_servers

ntp_servers:
  - 0.pool.ntp.org
  - 1.pool.ntp.org
  - 2.pool.ntp.org
  - 3.pool.ntp.org

# listen on ipv4 and/or ipv6
ntp_listen_on_v4: true
ntp_listen_on_v6: true

# allow all hosts in the inventory to
ntp_clients_inventory_access: true
ntp_clients: []
#  - name: HOSTNAME/IP
#    access: "" # empty or "nomodify notrap" etc.

ntp_driftfile_directory: "/var/lib/ntp"

# for custom configuration
ntp_custom_config: ""

```

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

Apache 2.0

Author Information
------------------

If you have problems with the role, feel free to create an issue on Github or contact me by mail.
