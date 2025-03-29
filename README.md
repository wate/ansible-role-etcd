etcd
=================

Setup etcd(work in progress)

OS Platform
-----------------

### Debian

- bookworm
- bullseye

Role Variables
--------------

### [defaults/main.yml](defaults/main.yml)

設定方法の詳細については[defaults/main.yml](defaults/main.yml)のサンプルコードなどを参照してください。

#### `etcd_packages`

インストールするパッケージ

### [vars/main.yml](vars/main.yml)

設定値については[vars/main.yml](vars/main.yml)を参照してください。

#### `etcd_dependency_packages`

#### `etcd_home`

#### `etcd_user`

#### `etcd_group`

Example Playbook
--------------

```yaml
- hosts: servers
  roles:
    - role: etcd
```

License
--------------

Apache License 2.0
