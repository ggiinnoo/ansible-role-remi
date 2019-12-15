Remi repo
=========

This role is used to setup the remi repository for centos

Requirements
------------

There are no requirements as of yet

Role Variables
--------------

The most imported variable is:

```
# List of all the repos
remiCentosRepoList:
  - name: remi-glpi91
  - name: remi-glpi92
  - name: remi-glpi93
  - name: remi-glpi94
  - name: remi-modular
  - name: remi-php54
  - name: remi-php70
  - name: remi-php71
  - name: remi-php72
  - name: remi-php73
  - name: remi-php74
  - name: remi
  - name: remi-safe
    state: enable
```

This lets you enable or disable an repo.
The standard vallue is disable


Dependencies
------------

There are no requirements for this installation

Example Playbook
----------------

    - name: remi repo install
      hosts: all
      roles:
        - ggiinnoo.remi

Upcomming features:
-------

License
-------

BSD

Author Information
------------------

    Creator: Gino Jansen
    Website: www.ginojansen.nl