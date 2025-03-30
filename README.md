etcd
=================

Setup etcd

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

#### `etcd_client_port`

etcdのクライアントポート  
@see https://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.txt

#### `etcd_server_port`

etcdのサーバーポート  
@see https://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.txt

#### `etcd_envs`

etcdの環境変数の設定  
@see https://etcd.io/docs/v3.5/op-guide/configuration/

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
