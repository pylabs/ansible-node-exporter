node_exporter
=============

This role is used to install node exporter automatically.

Role Variables
--------------

```yaml
node_exporter_version: NODE_EXPORTER_VERSION
node_exporter_base_dir: NODE_EXPORTER_BASE_DIR (default: /opt/node_exporter)
node_exporter_listen_address: NODE_EXPORTER_LISTEN_ADDRESS (default: 0.0.0.0)
node_exporter_listen_port: NODE_EXPORTER_LISTEN_PORT (default: 9100)
```

Dependencies
------------

- pylabs.sysbase

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
    - role: pylabs.node_exporter
  vars:
    node_exporter_version: "1.0.1"
```

License
-------

MIT

Author Information
------------------

William Wu <william@pylabs.org>
