Role Name
=========

Роль для установки [Lighthouse](https://github.com/VKCOM/lighthouse) - легковесный GUI для Clickhouse

Requirements
------------

- **Ansible 2.11+**

Role Variables
--------------

| Scope    | Variable                 | Default                                 | Description                            |
|----------|--------------------------|-----------------------------------------|----------------------------------------|
| defaults | role_lighthouse_location | /var/www/lighthouse                     | Расположение файлов сервера Lighthouse |
| vars     | role_lighthouse_vcs      | https://github.com/VKCOM/lighthouse.git | Ссылка на git-репозиторий              |

Dependencies
------------

| Role           | Source                                         | Description                                                   |
|----------------|------------------------------------------------|---------------------------------------------------------------|
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
