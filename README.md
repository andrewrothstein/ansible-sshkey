andrewrothstein.sshkey
=========
![Build Status](https://github.com/andrewrothstein/ansible-sshkey/actions/workflows/build.yml/badge.svg)

Installs a CA certificate, a host certificate, and a host private key onto the target hosts filesystem

Requirements
------------

See [meta/main.yml](meta/main.yml)

Role Variables
--------------

See [defaults/main.yml](defaults/main.yml)

Dependencies
------------

See [meta/main.yml](meta/main.yml)

Example Playbook
----------------

```yml
- hosts: servers
  roles:
    - role: andrewrothstein.sshkey
      sshkey_pki_dir: ~/super-secret/my-cluster-pki
      sshkey_target_dir: /etc/target-app
```

License
-------

MIT

Author Information
------------------

Andrew Rothstein <andrew.rothstein@gmail.com>
