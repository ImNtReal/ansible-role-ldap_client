Role Name
=========

Setup Arch Linux as a LDAP client with basic configuration.

Requirements
------------

A working LDAP server.

Role Variables
--------------

## Set in defaults
# Sets the default LDAP protocol to use to ldaps
ldap_protocol: ldaps

## Others
# Sets LDAP search base
ldap_base: dc=example,dc=com
# Sets LDAP server
ldap_server: ldap.example.com

Example Playbook
----------------

    - hosts: clients
      roles:
         - { role: imntreal.ldap_client }

License
-------

GPLv3

Author Information
------------------

Jameson Pugh <imntreal@gmail.com>
