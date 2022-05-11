tomcat_server
=========

This role can be used to install tomcat

[![CI](https://github.com/Rheinwerk/ansible-role-tomcat_server/actions/workflows/ci.yml/badge.svg)](https://github.com/Rheinwerk/ansible-role-tomcat_server/workflows/ci.yml)


Requirements
------------

None.

Role Variables
--------------

There is one main variable that drives this role: `_tomcat`. It is a map that contains all configuration and settings for this role.
Please see [defaults file][defaults].

[defaults]: defaults/main.yml

Dependencies
------------

None

Example Playbook
----------------

```yaml
- hosts: servers
  var:
    TOMCAT:
      ...
  roles:
     - { role: tomcat_server, tags: [ 'tomcat' ], _tomcat: "{{ TOMCAT }}" }

```

License
-------

Please see LICENSE.

Author Information
------------------

Original author is [Michael Schmitz](https://github.com/eifelmicha) as member of the [Rheinwerk](https://github.com/Rheinwerk) project.
