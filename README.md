Role Name
=========

Роль для установки [Lighthouse](https://github.com/VKCOM/lighthouse) - легковесный GUI для Clickhouse

Requirements
------------

- **Ansible 2.11+**

Role Variables
--------------

| Scope | Variable | Default | Description |
| ---- |---- | ---- | ---- |
| defaults | lighthouse_location | /var/www/lighthouse | Расположение  |
| vars | lighthouse_vcs | https://github.com/VKCOM/lighthouse.git | Ссылка на git-репозиторий |

Dependencies
------------

\-

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
