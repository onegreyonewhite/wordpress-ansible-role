wordpress_lamp_server
=========

This Ansible role for easy deploy latest wordpress with simple lamp on server.
Demo role for Polemarch Demo Project.

Requirements
------------

Nothing.

Role Variables
--------------

See default variables: `defaults/main.yml`

```yaml
wp_mysql_db: wordpress
```
MySQL db name for wordpress installation. 

```yaml
wp_mysql_user: wordpress
``` 
MySQL user for access to WP db. By default getting from `wp_mysql_db`.

```yaml
wp_mysql_password: wordpress
```
MySQL user password for access to WP db.
By default getting from `wp_mysql_user`.

```yaml
extra_redhat_packages: []
extra_ubuntu_packages: []
```
This vars setup extra packages needed for lamp server.
It could be php extra packages or additional apache modules.

Example Playbook
----------------

        - hosts: servers
          roles:
             - { role: onegreyonewhite.wordpress_lamp_server }

License
-------

BSD

Author Information
------------------

[Sergey Klyuykov](https://github.com/onegreyonewhite)