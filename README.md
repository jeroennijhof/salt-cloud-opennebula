salt-cloud-opennebula
=====================

This is the opennebula provider for salt-cloud.
With this provider it's possible to use salt-cloud commands against an opennebula based cloud.

Provider example
----------------

```
provider:
  xml_rpc: http://localhost:2633
  user: oneadmin
  password: whatever
  provider: opennebula
```

Profile example
---------------
Note: Images refer to opennebula templates.

```
debian:
  provider: baarn
  image: Debian 7.4.0
  ssh_username: debian
  ssh_key_file: '/etc/salt/id_rsa.debian'
  sudo: True
  tty: True
```

