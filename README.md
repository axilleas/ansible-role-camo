ansible-role-camo
=========

Camo, an http proxy to route images through SSL.

Requirements
------------

The only requirement is `nodejs`. For RHEL/CentOS you must enable the EPEL
repository.

Role Variables
--------------

Camo recieves user defined settings with environmental variables as seen in
<https://github.com/atmos/camo/tree/master#configuration>. You can find their
default values in `defaults/main.yml` which are then loaded via the template
`camo.env.j2` in systemd service.

Example Playbook
----------------

```
- hosts: servers
  roles:
     - { role: librenet.ansible-role-camo }
```

License
-------

MIT

Author Information
------------------

Achilleas Pipinellis (http://axilleas.me)
