Role Name
=========

Set Hostname and Fully Qualified Name

Requirements
------------

None

Role Variables
--------------

- fqn_hostname: Hostname. Example:'web1'
- fqn_only_hostname: Set only hostname and not modify /etc/hosts file. Example: false
- fqn_full: Fully qualified name. Example:'web1.mydomain.com'
- fqn_ip: Ip addres of hostname. Example:'54.54.54.54'


Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      vars:
        fqn_hostname: 'web1'
        fqn_full: 'web1.mydomain.com'
        fqn_ip: '54.54.54.54'
      roles:
         - fqn

License
-------

BSD

Author Information
------------------

Antonio Barbaro <antonio.barbaro@gmail.com>
