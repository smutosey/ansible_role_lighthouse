Role Name
=========

Роль для установки [Lighthouse](https://github.com/VKCOM/lighthouse) - легковесный GUI для Clickhouse

Requirements
------------

- **Ansible 2.11+**

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

| Role | Source | Description |
| ---- | ---- | ---- |
| nginxinc.nginx | git@github.com:nginxinc/ansible-role-nginx.git | Роль для инсталляции Nginx, необходим для запуска веб-сервера |

Example Playbook
----------------

Пример использования роли:

```yaml
- name: Install Lighthouse
  hosts: lighthouse
  become: true
  roles:
    - lighthouse
  tags: lighthou se
```

License
-------

MIT License.
